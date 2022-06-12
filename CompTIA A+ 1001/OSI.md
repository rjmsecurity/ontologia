# OSI layers

> All People Seem To Need Data Processing

Layer | Data | Headers | Protocols | Hardware
-- | - | - | - | -
7 – Application | data
6 – Presentation | data
5 – Session | data
4 – Transport | segment (TCP), datagram (UDP) | TCP header
3 – Network | packet | IP header |  | router, multilayer switch
2 – Data link | frame | MAC header & trailer |  | switch, bridge
1 – Physical | bits |  |  | ethernet cable, hub

- this is just a model to think about how data flows, the *protocol suite* today is actually TCP/IP