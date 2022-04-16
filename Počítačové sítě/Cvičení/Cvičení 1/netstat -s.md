[kevin.danek@a0307 ~]$ netstat -s
Ip:
    9218048 total packets received
    0 forwarded
    0 incoming packets discarded
    5844695 incoming packets delivered
    2538800 requests sent out
    16 dropped because of missing route
    2 fragments dropped after timeout
    52 reassemblies required
    25 packets reassembled ok
    2 packet reassembles failed
Icmp:
    23890 ICMP messages received
    1231 input ICMP message failed.
    ICMP input histogram:
        destination unreachable: 12454
        timeout in transit: 5
        echo requests: 10194
        echo replies: 10
        timestamp request: 2
    61961 ICMP messages sent
    0 ICMP messages failed
    ICMP output histogram:
        destination unreachable: 51765
        echo replies: 10194
        timestamp replies: 2
IcmpMsg:
        InType0: 10
        InType3: 12454
        InType8: 10194
        InType9: 1225
        InType11: 5
        InType13: 2
        OutType0: 10194
        OutType3: 51765
        OutType14: 2
Tcp:
    6249 active connections openings
    12 passive connection openings
    0 failed connection attempts
    128 connection resets received
    9 connections established
    5767021 segments received
    10441835 segments send out
    5362 segments retransmited
    1 bad segments received.
    605 resets sent
Udp:
    53758 packets received
    9 packets to unknown port received.
    0 packet receive errors
    58983 packets sent
    0 receive buffer errors
    0 send buffer errors
UdpLite:
TcpExt:
    3480 TCP sockets finished time wait in fast timer
    37684 delayed acks sent
    6 delayed acks further delayed because of locked socket
    Quick ack mode was activated 99 times
    93 packets directly queued to recvmsg prequeue.
    5020 bytes directly in process context from backlog
    61144 bytes directly received in process context from prequeue
    1894745 packet headers predicted
    41 packets header predicted and directly queued to user
    30431 acknowledgments not containing data payload received
    4620994 predicted acknowledgments
    168 times recovered from packet loss by selective acknowledgements
    6 congestion windows recovered without slow start by DSACK
    15 congestion windows recovered without slow start after partial ack
    TCPLostRetransmit: 107
    6 timeouts after SACK recovery
    1521 fast retransmits
    69 forward retransmits
    58 retransmits in slow start
    886 other TCP timeouts
    TCPLossProbes: 188
    TCPLossProbeRecovery: 136
    8 SACK retransmits failed
    99 DSACKs sent for old packets
    3 DSACKs sent for out of order packets
    164 DSACKs received
    201 connections reset due to unexpected data
    61 connections reset due to early user close
    3 connections aborted due to timeout
    TCPDSACKIgnoredNoUndo: 26
    TCPSpuriousRTOs: 1
    TCPSackShifted: 6602
    TCPSackMerged: 2917
    TCPSackShiftFallback: 1543
    IPReversePathFilter: 14126
    TCPRcvCoalesce: 213676
    TCPOFOQueue: 12206
    TCPOFOMerge: 3
    TCPChallengeACK: 1
    TCPSYNChallenge: 1
    TCPSpuriousRtxHostQueues: 344
    TCPAutoCorking: 164881
    TCPFromZeroWindowAdv: 10
    TCPToZeroWindowAdv: 10
    TCPWantZeroWindowAdv: 17
    TCPSynRetrans: 3411
    TCPOrigDataSent: 9374364
    TCPHystartTrainDetect: 21
    TCPHystartTrainCwnd: 583
    TCPHystartDelayDetect: 1
    TCPHystartDelayCwnd: 97
IpExt:
    InNoRoutes: 1
    InMcastPkts: 1103599
    OutMcastPkts: 949
    InBcastPkts: 2214880
    OutBcastPkts: 24
    InOctets: 8821762723
    OutOctets: 12362039786
    InMcastOctets: 122105508
    OutMcastOctets: 132038
    InBcastOctets: 223373129
    OutBcastOctets: 1872
    InNoECTPkts: 13832052
    InECT0Pkts: 23
    InCEPkts: 2