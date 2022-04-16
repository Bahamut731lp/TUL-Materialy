# Cvičení 3
```bash
ifconfig

p2p1: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.1.114  netmask 255.255.255.0  broadcast 192.168.1.255
        inet6 fdb7:3f96:41e6:0:5131:ab32:f95a:48ce  prefixlen 64  scopeid 0x0<global>
        inet6 fe80::8060:e8f:5a82:9f9a  prefixlen 64  scopeid 0x20<link>
        inet6 fd03:8b53:4d8b:c:d366:dde7:1de8:3ea  prefixlen 64  scopeid 0x0<global>
        inet6 fdb7:3f96:41e6::8a8  prefixlen 128  scopeid 0x0<global>
        inet6 fd03:8b53:4d8b:c::8a8  prefixlen 128  scopeid 0x0<global>
        ether b4:96:91:26:1a:8d  txqueuelen 1000  (Ethernet)
        RX packets 1509  bytes 991126 (967.8 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1152  bytes 157316 (153.6 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        device memory 0xee100000-ee1fffff

vboxnet0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.56.1  netmask 255.255.255.0  broadcast 192.168.56.255
        inet6 fe80::800:27ff:fe00:0  prefixlen 64  scopeid 0x20<link>
        ether 0a:00:27:00:00:00  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 173  bytes 9897 (9.6 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```

```bash
[kevin.danek@a0313 ~]$ curl ifconfig.me
147.230.78.84

[kevin.danek@a0313 ~]$ nslookup 147.230.78.84
84.78.230.147.in-addr.arpa      name = a0313.nti.tul.cz.

```

```bash
[kevin.danek@a0313 ~]$ arp
Address                  HWtype  HWaddress           Flags Mask            Iface
192.168.56.109                   (incomplete)                              vboxnet0
192.168.56.101                   (incomplete)                              vboxnet0
192.168.56.121                   (incomplete)                              vboxnet0
192.168.56.125                   (incomplete)                              vboxnet0
192.168.56.113                   (incomplete)                              vboxnet0
192.168.56.117                   (incomplete)                              vboxnet0
192.168.56.139                   (incomplete)                              vboxnet0
192.168.56.143                   (incomplete)                              vboxnet0
192.168.56.131                   (incomplete)                              vboxnet0
192.168.56.135                   (incomplete)                              vboxnet0
192.168.56.147                   (incomplete)                              vboxnet0
a0300.nti.tul.cz         ether   54:bf:64:62:cb:51   C                     enp0s31f6
192.168.56.106                   (incomplete)                              vboxnet0
a0304.nti.tul.cz         ether   54:bf:64:62:ce:c1   C                     enp0s31f6
192.168.56.110                   (incomplete)                              vboxnet0
192.168.56.102                   (incomplete)                              vboxnet0
192.168.56.122                   (incomplete)                              vboxnet0
192.168.56.126                   (incomplete)                              vboxnet0
192.168.56.114                   (incomplete)                              vboxnet0
192.168.56.118                   (incomplete)                              vboxnet0
share.nti.tul.cz         ether   10:98:36:a2:75:fb   C                     enp0s31f6
192.168.56.136                   (incomplete)                              vboxnet0
192.168.56.140                   (incomplete)                              vboxnet0
gateway                  ether   cc:2d:e0:e7:8d:3f   C                     p2p1
192.168.56.128                   (incomplete)                              vboxnet0
192.168.56.132                   (incomplete)                              vboxnet0
192.168.56.144                   (incomplete)                              vboxnet0
router-b.tul.cz          ether   d0:c7:89:a9:d2:80   C                     enp0s31f6
192.168.56.148                   (incomplete)                              vboxnet0
192.168.56.107                   (incomplete)                              vboxnet0
192.168.56.111                   (incomplete)                              vboxnet0
192.168.56.103                   (incomplete)                              vboxnet0
192.168.56.123                   (incomplete)                              vboxnet0
192.168.56.127                   (incomplete)                              vboxnet0
192.168.56.115                   (incomplete)                              vboxnet0
192.168.56.119                   (incomplete)                              vboxnet0
192.168.56.137                   (incomplete)                              vboxnet0
192.168.56.141                   (incomplete)                              vboxnet0
192.168.56.129                   (incomplete)                              vboxnet0
192.168.56.133                   (incomplete)                              vboxnet0
192.168.56.145                   (incomplete)                              vboxnet0
192.168.56.149                   (incomplete)                              vboxnet0
192.168.56.104                   (incomplete)                              vboxnet0
192.168.56.108                   (incomplete)                              vboxnet0
192.168.56.100           ether   08:00:27:d3:8f:71   C                     vboxnet0
192.168.56.120                   (incomplete)                              vboxnet0
192.168.56.124                   (incomplete)                              vboxnet0
192.168.56.112                   (incomplete)                              vboxnet0
192.168.56.116                   (incomplete)                              vboxnet0
192.168.56.138                   (incomplete)                              vboxnet0
192.168.56.142                   (incomplete)                              vboxnet0
192.168.56.130                   (incomplete)                              vboxnet0
192.168.56.134                   (incomplete)                              vboxnet0
192.168.56.146                   (incomplete)                              vboxnet0
192.168.56.150                   (incomplete)                              vboxnet0
192.168.56.105                   (incomplete)                              vboxnet0
```

`192.168.56.100` je aktivní.

## Virtuál
```bash
student@virta0313:~$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 08:00:27:10:1c:18 brd ff:ff:ff:ff:ff:ff
    inet 10.0.2.15/24 brd 10.0.2.255 scope global noprefixroute dynamic enp0s3
       valid_lft 86207sec preferred_lft 86207sec
    inet6 fe80::cbcc:6509:cedb:d67c/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
3: enp0s8: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 08:00:27:29:4a:dc brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.188/24 brd 192.168.1.255 scope global noprefixroute dynamic enp0s8
       valid_lft 43007sec preferred_lft 43007sec
    inet6 fdb7:3f96:41e6::f8d/128 scope global noprefixroute
       valid_lft forever preferred_lft forever
    inet6 fd03:8b53:4d8b:c::f8d/128 scope global noprefixroute
       valid_lft forever preferred_lft forever
    inet6 fdb7:3f96:41e6:0:7c7b:2332:da3e:de87/64 scope global noprefixroute
       valid_lft forever preferred_lft forever
    inet6 fd03:8b53:4d8b:c:283f:c873:9a3c:ce6e/64 scope global noprefixroute
       valid_lft forever preferred_lft forever
    inet6 fe80::fc66:9911:e26e:b897/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
4: enp0s9: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 08:00:27:d3:8f:71 brd ff:ff:ff:ff:ff:ff
    inet 192.168.56.100/24 brd 192.168.56.255 scope global noprefixroute dynamic enp0s9
       valid_lft 1007sec preferred_lft 1007sec
    inet6 fe80::90e:c1f7:4060:fa67/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
```

```bash
student@virta0313:~$ curl ifconfig.me
147.230.78.84

student@virta0313:~$ nslookup 147.230.78.84
84.78.230.147.in-addr.arpa      name = a0313.nti.tul.cz.

Authoritative answers can be found from:

student@virta0313:~$ ip route
default via 10.0.2.2 dev enp0s3 proto dhcp metric 100
default via 192.168.1.1 dev enp0s8 proto dhcp metric 101
10.0.2.0/24 dev enp0s3 proto kernel scope link src 10.0.2.15 metric 100
192.168.1.0/24 dev enp0s8 proto kernel scope link src 192.168.1.188 metric 101
192.168.56.0/24 dev enp0s9 proto kernel scope link src 192.168.56.100 metric 102


student@virta0313:~$ sudo ip route del default via 192.168.1.1

student@virta0313:~$ ip route list
default via 10.0.2.2 dev enp0s3 proto dhcp metric 100
10.0.2.0/24 dev enp0s3 proto kernel scope link src 10.0.2.15 metric 100
192.168.1.0/24 dev enp0s8 proto kernel scope link src 192.168.1.188 metric 101
192.168.56.0/24 dev enp0s9 proto kernel scope link src 192.168.56.100 metric 102

student@virta0313:~$ ip route add default via 192.168.1.1 metric 99

student@virta0313:~$ ip route list
default via 192.168.1.1 dev enp0s8 metric 99
default via 10.0.2.2 dev enp0s3 proto dhcp metric 100
10.0.2.0/24 dev enp0s3 proto kernel scope link src 10.0.2.15 metric 100
192.168.1.0/24 dev enp0s8 proto kernel scope link src 192.168.1.188 metric 101
192.168.56.0/24 dev enp0s9 proto kernel scope link src 192.168.56.100 metric 102

student@virta0313:~$ curl ifconfig.me
147.230.78.154

student@virta0313:~$ nslookup 147.230.78.154
154.78.230.147.in-addr.arpa     name = a03r03.nti.tul.cz.

Authoritative answers can be found from:

```