# OSI Model Layers

Layer | Layer Name | Data Type | Headers/trailers | Hardware
-- | - | - | - | -
7 | Application | Data
6 | Presentation | Data
5 | Session | Data
4 | Transport | Segment (TCP)<br>Datagram (UDP) | TCP header
3 | Network | Packet | IP header | Router<br>Multilayer switch
2 | Data link | Frame | MAC header<br>MAC trailer | Switch<br>Bridge
1 | Physical | Bit |  | Ethernet cable<br>Hub

- All People Seem To Need Data Processing
- This is just a model to think about how data flows, the *protocol suite* today is actually TCP/IP