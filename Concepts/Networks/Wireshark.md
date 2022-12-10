# Wireshark

- packet capture app giving a practical view of the OSI model
- top window shows summary where each list item is a particular frame that's traveling across the network
- at the bottom is a hex and ASCII representation of the data
- middle window shows details for a frame with the communication broken down by OSI layer
- e.g. *Frame 88 (2005 bytes on the wire)* is describing traffic being received at layer 1
- line 2, *Ethernet II, Src: 00:21:70:6f:06:f2, Dst: 00:09:5b:d4:bb:fe* describes layer 2
- line 3, *Internet Protocol, Src: 192.168.0.8, Dst: 72.14.247.19* describes layer 3
- line 4, *Transmission Control Protocol, Src Port: 18429, Dst Port: 443* describes layer 4
- line 5, *Secure Socket Layer* describes layers 5, 6, 7 (commonly grouped)

#networkplus **objective 1.1** *Compare and contrast the Open Systems Interconnection (OSI) model layers and encapsulation concepts.*
