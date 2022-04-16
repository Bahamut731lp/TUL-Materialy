# Směrování routeru

```bash
# Zapnutí DHCP na druhé síťovce
student@virta0313:~$ sudo ip addr add 192.168.1.60/24 dev enp0s8
student@virta0313:~$ sudo ip route add default via 192.168.1.1 dev enp0s8


[kevin.danek@a0313 ~]$ sudo ifup p2p1
[kevin.danek@a0313 ~]$ ifdown p2p1

student@virta0313:~$ sudo dhclient -r enp0s8
student@virta0313:~$ dhclient enp0s8

[kevin.danek@a0313 ~]$ curl ifconfig.me
147.230.78.84

[kevin.danek@a0313 ~]$ ping 8.8.8.8
--- 8.8.8.8 ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2003ms

[kevin.danek@a0313 ~]$ arp
Address                  HWtype  HWaddress           Flags Mask            Iface
gateway                  ether   cc:2d:e0:e7:8d:3f   C                     p2p1
router-b.tul.cz          ether   d0:c7:89:a9:d2:80   C                     enp0s31f6
192.168.56.100           ether   08:00:27:b7:e8:08   C                     vboxnet0
a0300.nti.tul.cz         ether   54:bf:64:62:cb:51   C                     enp0s31f6
share.nti.tul.cz         ether   10:98:36:a2:75:fb   C                     enp0s31f6

```

```bash
config redirect
	option	name		'DNAT WAN to LAN for SSH'
	option	src		'wan'
	option	src_dport	'19900'
	option	dest		'lan'
	option	dest_ip		'192.168.1.1'
	option	dest_port	'22'
	option	proto		'tcp'
	option	target		'DNAT'
```