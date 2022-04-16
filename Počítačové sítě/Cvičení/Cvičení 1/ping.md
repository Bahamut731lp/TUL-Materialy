[kevin.danek@a0307 ~]$ ping -s 1024B -c 5 www.tul.cz
PING novy.tul.cz (147.230.18.195) 1024(1052) bytes of data.
1032 bytes from novy.tul.cz (147.230.18.195): icmp_seq=1 ttl=63 time=0.409 ms
1032 bytes from novy.tul.cz (147.230.18.195): icmp_seq=2 ttl=63 time=0.422 ms
1032 bytes from novy.tul.cz (147.230.18.195): icmp_seq=3 ttl=63 time=0.460 ms
1032 bytes from novy.tul.cz (147.230.18.195): icmp_seq=4 ttl=63 time=0.460 ms
1032 bytes from novy.tul.cz (147.230.18.195): icmp_seq=5 ttl=63 time=0.527 ms

--- novy.tul.cz ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4000ms
rtt min/avg/max/mdev = 0.409/0.455/0.527/0.047 ms

[kevin.danek@a0307 ~]$ ping -s 1024B -c 5 www.seznam.cz
PING www.seznam.cz (77.75.75.176) 1024(1052) bytes of data.
1032 bytes from 77.75.75.176 (77.75.75.176): icmp_seq=1 ttl=57 time=3.77 ms
1032 bytes from 77.75.75.176 (77.75.75.176): icmp_seq=2 ttl=57 time=3.99 ms
1032 bytes from 77.75.75.176 (77.75.75.176): icmp_seq=3 ttl=57 time=3.90 ms
1032 bytes from 77.75.75.176 (77.75.75.176): icmp_seq=4 ttl=57 time=4.00 ms
1032 bytes from 77.75.75.176 (77.75.75.176): icmp_seq=5 ttl=57 time=3.99 ms

--- www.seznam.cz ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4005ms
rtt min/avg/max/mdev = 3.773/3.935/4.001/0.088 ms

[kevin.danek@a0307 ~]$ ping -s 1024B -c 5 www.google.cz
PING www.google.cz (142.251.36.67) 1024(1052) bytes of data.
76 bytes from prg03s10-in-f3.1e100.net (142.251.36.67): icmp_seq=1 ttl=59 (truncated)
76 bytes from prg03s10-in-f3.1e100.net (142.251.36.67): icmp_seq=2 ttl=59 (truncated)
76 bytes from prg03s10-in-f3.1e100.net (142.251.36.67): icmp_seq=3 ttl=59 (truncated)
76 bytes from prg03s10-in-f3.1e100.net (142.251.36.67): icmp_seq=4 ttl=59 (truncated)
76 bytes from prg03s10-in-f3.1e100.net (142.251.36.67): icmp_seq=5 ttl=59 (truncated)

--- www.google.cz ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4008ms
rtt min/avg/max/mdev = 3.645/3.808/3.873/0.099 ms

[kevin.danek@a0307 ~]$ ping -s 1024B -c 5 www.facebook.com
PING star-mini.c10r.facebook.com (157.240.30.35) 1024(1052) bytes of data.
1032 bytes from edge-star-mini-shv-01-prg1.facebook.com (157.240.30.35): icmp_seq=1 ttl=57 time=3.67 ms
1032 bytes from edge-star-mini-shv-01-prg1.facebook.com (157.240.30.35): icmp_seq=2 ttl=57 time=3.89 ms
1032 bytes from edge-star-mini-shv-01-prg1.facebook.com (157.240.30.35): icmp_seq=3 ttl=57 time=3.87 ms
1032 bytes from edge-star-mini-shv-01-prg1.facebook.com (157.240.30.35): icmp_seq=4 ttl=57 time=3.74 ms
1032 bytes from edge-star-mini-shv-01-prg1.facebook.com (157.240.30.35): icmp_seq=5 ttl=57 time=3.89 ms

--- star-mini.c10r.facebook.com ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4006ms
rtt min/avg/max/mdev = 3.670/3.815/3.894/0.120 ms

maximální veikost ping packetu je 65535B (2^16)