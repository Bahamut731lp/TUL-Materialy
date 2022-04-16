# Konfigurace LAN

## Ruční konfigurace
```bash
ssh a0313.nti.tul.cz -l kevin.danek
ssh 192.168.56.100 -l student

ip a
sudo ip addr add 192.168.1.60/24 dev enp0s8
ip a

ip route
sudo ip route add default via 192.168.1.1
ip route
```

```bash
ssh a0313.nti.tul.cz -l kevin.danek
ssh 192.168.56.100 -l student

(ip a; [sudo ip addr add 192.168.1.60/24 dev enp0s8]()) | diff - <(ip a)
ping 192.168.1.1 -c 4 | grep "packets transmitted"
```

```bash
student@virta0313:~$ diff -u <(ip a) <(sudo ip addr add 192.168.1.60/24 dev enp0s8; ip a)
--- /dev/fd/63  2022-04-04 13:17:31.419000000 +0200
+++ /dev/fd/62  2022-04-04 13:17:31.419000000 +0200
@@ -12,6 +12,8 @@
        valid_lft forever preferred_lft forever
 3: enp0s8: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
     link/ether 08:00:27:4a:15:37 brd ff:ff:ff:ff:ff:ff
+    inet 192.168.1.60/24 scope global enp0s8
+       valid_lft forever preferred_lft forever
     inet6 fdb7:3f96:41e6::f8d/128 scope global noprefixroute
        valid_lft forever preferred_lft forever
     inet6 fd03:8b53:4d8b:c::f8d/128 scope global noprefixroute
```

```bash
student@virta0313:~$ diff -u <(ip route) <(sudo ip route add default via 192.168.1.1 metric 99; ip route)
--- /dev/fd/63  2022-04-04 13:16:11.210000000 +0200
+++ /dev/fd/62  2022-04-04 13:16:11.210000000 +0200
@@ -1,3 +1,4 @@
+default via 192.168.1.1 dev enp0s8 metric 99
 default via 10.0.2.2 dev enp0s3 proto dhcp metric 100
 10.0.2.0/24 dev enp0s3 proto kernel scope link src 10.0.2.15 metric 100
 192.168.1.0/24 dev enp0s8 proto kernel scope link src 192.168.1.60
```

```bash
student@virta0313:~$ ping 192.168.1.1 -c 4 | grep "packets transmitted"
4 packets transmitted, 4 received, 0% packet loss, time 3002ms
```

## Automatická konfigurace
```bash
ssh 192.168.1.1 -l root

#Jestli existuje DHCP
service | grep "dhcp"
#Jestli DHPC frčí:
ps | grep -v "grep" | grep "dhcp"

#DHCP Config
OG=$(cat /etc/config/dhcp)

#Edit Config
nano /etc/config/dhcp

#Diff změn
diff <(echo "$OG") <(cat /etc/config/dhcp)

#Restart DHCP
service odhcpd restart

#Odejití z routeru
exit

#Nastavení DHCP na
dhclient eth0 -v
```

```bash
root@a03r03: service | grep "dhcp"
odhcpd

root@a03r03:~# ps | grep -v "grep" | grep "dhcp"
 1154 root      1444 S    /usr/sbin/odhcpd
 1411 root      1208 S    udhcpc -p /var/run/udhcpc-eth0.2.pid -s /lib/netifd/dhcp.script -f -t 0 -i eth0.2 -x hostnam
 1414 root      1048 S    odhcp6c -s /lib/netifd/dhcpv6.script -P0 -t120 eth0.2


#Původní
config dnsmasq option domainneeded '1' option boguspriv '1' option filterwin2k '0' option localise_queries '1' option rebind_protection '1' option rebind_localhost '1' option local '/lan/' option domain 'lan' option expandhosts '1' option nonegcache '0' option authoritative '1' option readethers '1' option leasefile '/tmp/dhcp.leases' option resolvfile '/tmp/resolv.conf.auto' option nonwildcard '1' option localservice '1' config dhcp 'lan' option interface 'lan' option start '100' option limit '150' option leasetime '12h' option dhcpv6 'server' option ra 'server' config dhcp 'wan' option interface 'wan' option ignore '1' config odhcpd 'odhcpd' option maindhcp '0' option leasefile '/tmp/hosts/odhcpd' option leasetrigger '/usr/sbin/odhcpd-update' option loglevel '4'

#Nový
config dhcp 'lan'
        option interface 'lan'
        option start '50'
        option limit '100'
        option leasetime '12h'
        option dhcpv6 'server'
        option ra 'server'

root@a03r03:~# service dnsmasq reload
udhcpc: started, v1.30.1
udhcpc: sending discover
udhcpc: no lease, failing

exit

ifconfig enp0s8 down
ifconfig enp0s8 up
sudo ip route del default via 192.168.1.1
sudo ip route add default via 192.168.1.1 metric 99

enp0s8: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 08:00:27:4a:15:37 brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.91/24 brd 192.168.1.255 scope global noprefixroute dynamic enp0s8
       valid_lft 43198sec preferred_lft 43198sec

student@virta0313:~$ iperf3 -s -B 192.168.1.91
-----------------------------------------------------------
Server listening on 5201
-----------------------------------------------------------
Accepted connection from 192.168.1.122, port 54264
[  5] local 192.168.1.91 port 5201 connected to 192.168.1.122 port 54266
[ ID] Interval           Transfer     Bandwidth
[  5]   0.00-1.00   sec   105 MBytes   883 Mbits/sec
[  5]   1.00-2.00   sec   112 MBytes   941 Mbits/sec
[  5]   2.00-3.00   sec   112 MBytes   941 Mbits/sec
[  5]   3.00-4.00   sec   112 MBytes   941 Mbits/sec
[  5]   4.00-5.00   sec   112 MBytes   941 Mbits/sec
[  5]   5.00-6.00   sec   112 MBytes   941 Mbits/sec
[  5]   6.00-7.00   sec   112 MBytes   941 Mbits/sec
[  5]   7.00-8.00   sec   112 MBytes   941 Mbits/sec
[  5]   8.00-9.00   sec   112 MBytes   941 Mbits/sec
[  5]   9.00-10.00  sec   112 MBytes   941 Mbits/sec
[  5]  10.00-10.03  sec  3.86 MBytes   939 Mbits/sec
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bandwidth
[  5]   0.00-10.03  sec  0.00 Bytes  0.00 bits/sec                  sender
[  5]   0.00-10.03  sec  1.09 GBytes   936 Mbits/sec                  receiver

#Superiórní Daněk, Jiřina Halbyška, Matěj polská šunka, (Daun), Vít Machač
```
## Měření rychlosti
```bash
#Server
iperf3 -s

#Client
iperf3 -c
```