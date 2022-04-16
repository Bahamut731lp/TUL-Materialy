[kevin.danek@a0307 ~]$ ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: p2p1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP group default qlen 1000
    link/ether b4:96:91:26:1a:e9 brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.156/24 brd 192.168.1.255 scope global noprefixroute dynamic p2p1
       valid_lft 42820sec preferred_lft 42820sec
    inet6 fd03:8b53:4d8b:0:b696:91ff:fe26:1ae9/64 scope global mngtmpaddr dynamic
       valid_lft forever preferred_lft forever
    inet6 fe80::b696:91ff:fe26:1ae9/64 scope link
       valid_lft forever preferred_lft forever
3: enp0s31f6: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
    link/ether 54:bf:64:62:ce:4b brd ff:ff:ff:ff:ff:ff
    inet 147.230.78.78/21 brd 147.230.79.255 scope global noprefixroute dynamic enp0s31f6
       valid_lft 36532sec preferred_lft 36532sec
    inet6 fe80::7ffe:8963:bc14:f9ce/64 scope link tentative noprefixroute dadfailed
       valid_lft forever preferred_lft forever
    inet6 fe80::6671:3582:2c7e:c8ac/64 scope link tentative noprefixroute dadfailed
       valid_lft forever preferred_lft forever
    inet6 fe80::53df:8fde:4335:467/64 scope link tentative noprefixroute dadfailed
       valid_lft forever preferred_lft forever
4: wlp2s0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP group default qlen 1000
    link/ether 7c:2a:31:1f:63:23 brd ff:ff:ff:ff:ff:ff
    inet 192.168.174.82/21 brd 192.168.175.255 scope global noprefixroute dynamic wlp2s0
       valid_lft 429sec preferred_lft 429sec
    inet6 fe80::f252:f0a9:fda:77f6/64 scope link noprefixroute
       valid_lft forever preferred_lft forever
5: virbr0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN group default qlen 1000
    link/ether 52:54:00:b8:63:ee brd ff:ff:ff:ff:ff:ff
    inet 192.168.122.1/24 brd 192.168.122.255 scope global virbr0
       valid_lft forever preferred_lft forever
6: virbr0-nic: <BROADCAST,MULTICAST> mtu 1500 qdisc pfifo_fast master virbr0 state DOWN group default qlen 1000
    link/ether 52:54:00:b8:63:ee brd ff:ff:ff:ff:ff:ff
7: docker0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue state DOWN group default
    link/ether 02:42:4f:01:78:c4 brd ff:ff:ff:ff:ff:ff
    inet 172.17.0.1/16 scope global docker0
       valid_lft forever preferred_lft forever