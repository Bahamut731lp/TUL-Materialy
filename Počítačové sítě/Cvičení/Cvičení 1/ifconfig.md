[kevin.danek@a0307 ~]$ ifconfig
docker0: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        inet 172.17.0.1  netmask 255.255.0.0  broadcast 0.0.0.0
        ether 02:42:4f:01:78:c4  txqueuelen 0  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

enp0s31f6: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 147.230.78.78  netmask 255.255.248.0  broadcast 147.230.79.255
        inet6 fe80::7ffe:8963:bc14:f9ce  prefixlen 64  scopeid 0x20<link>
        inet6 fe80::6671:3582:2c7e:c8ac  prefixlen 64  scopeid 0x20<link>
        inet6 fe80::53df:8fde:4335:467  prefixlen 64  scopeid 0x20<link>
        ether 54:bf:64:62:ce:4b  txqueuelen 1000  (Ethernet)
        RX packets 22813958  bytes 9880534949 (9.2 GiB)
        RX errors 387  dropped 0  overruns 0  frame 309
        TX packets 10545882  bytes 12958855801 (12.0 GiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        device interrupt 20  memory 0xee300000-ee320000

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 12392  bytes 4411552 (4.2 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 12392  bytes 4411552 (4.2 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

p2p1: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.1.156  netmask 255.255.255.0  broadcast 192.168.1.255
        inet6 fd03:8b53:4d8b:0:b696:91ff:fe26:1ae9  prefixlen 64  scopeid 0x0<global>
        inet6 fe80::b696:91ff:fe26:1ae9  prefixlen 64  scopeid 0x20<link>
        ether b4:96:91:26:1a:e9  txqueuelen 1000  (Ethernet)
        RX packets 1898  bytes 327729 (320.0 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 344  bytes 49157 (48.0 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        device memory 0xee100000-ee1fffff

virbr0: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        inet 192.168.122.1  netmask 255.255.255.0  broadcast 192.168.122.255
        ether 52:54:00:b8:63:ee  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

wlp2s0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.174.82  netmask 255.255.248.0  broadcast 192.168.175.255
        inet6 fe80::f252:f0a9:fda:77f6  prefixlen 64  scopeid 0x20<link>
        ether 7c:2a:31:1f:63:23  txqueuelen 1000  (Ethernet)
        RX packets 59665  bytes 5644286 (5.3 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 51191  bytes 3875145 (3.6 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0