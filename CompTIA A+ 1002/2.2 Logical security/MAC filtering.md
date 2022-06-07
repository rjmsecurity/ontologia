> 2.2 Explain logical security concepts. 

# MAC filtering

- it's common to see MAC filtering in switches and WAPs
- network admin keeps a list of MAC addresses to be allowed or filtered from the network
- guests will have to have their MAC addresses added

- but anyone can use wireless LAN analysis to catch a packet going through the network and take its MAC address
- then configure their NIC to spoof the allowed MAC address
- for this reason MAC filtering is known as *security through obscurity*, because if someone does know your method, they can circumvent it