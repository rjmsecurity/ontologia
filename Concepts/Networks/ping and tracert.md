# `ping` and `tracert`

- send a device a `ping` to determine if it's operating and able to talk to you
- relies on ICMP
- primary troubleshooting tool
- it also determines the round trip time
- by default Windows performs four pings so you should receive four replies each with bytes, time, TTL

- `tracert` traces the route (get it? router...) that the ping takes to get to the device
- takes advantage of *ICMP Time to Live Exceeded error*: when TTL is zero, the packet is expired and has to be sent back
- so first a packet with TTL=1 is sent, the first router picks it up and decrements it to zero and has to sent it back: `1  2 ms  10.10.10.1`
- then a packet with TTL=2 is sent, the first router decrements it to 1, the second router decrements it to zero and sends it back: `2  1 ms  172.16.1.2`
- each time it gets one router further than before until it reaches the destination and the route is mapped
- the command performs three separate tests for each device so in the final output you'll see three time columns: `9 ms  8 ms  8 ms`
- note that sometimes the route changes, not all devices will reply with ICMP Time Exceeded messages, some firewalls will filter, etc. 
- in Linux/Unix/macOS you can change it to use UDP or TCP
- iOS devices send UDP datagrams over port 33434

#aplus #core2 **1.4** *Given a scenario, use appropriate Microsoft command line tools.* 
