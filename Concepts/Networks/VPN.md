# VPN concentrators and VPN connections
(part of the 1.8 section on establishing networking connections)

#### VPN concentrator

- an encrypted tunnel is created between your device and a VPN concentrator somewhere on the corporate network
- so it goes: your laptop at a cafe -> internet -> concentrator -> corporate network
- normally you, on the internet, wouldn't have access to the resources on the private network behind a firewall 
- people can snoop and see that you're communicating with the concentrator but the traffic is encrypted ✅
- the concentrator decrypts incoming traffic and sends it into the network and vice versa

#### VPN connections

- the OS comes with a built in client for configuring VPN connections: [Network and Sharing Center](Network%20and%20Sharing%20Center.md)
- it has options to add the internet address (e.g. an IP) and destination name (e.g. VPN Connection)
- then a checkbox to use a smart card if your laptop has a slot for one – MFA (know, have, are)
- once the configuration is created you can connect from the network status icon at the bottom of the screen
- just provide your credentials and you have an encrypted tunnel

#aplus #core2 **1.8** *Given a scenario, configure Microsoft Windows networking on a client/desktop.*
