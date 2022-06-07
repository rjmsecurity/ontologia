> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Wired connections
(part of the 1.8 section on establishing networking connections)

- also common, an ethernet connection
- [Network and Sharing Center](../1.6%20Control%20Panel/Network%20and%20Sharing%20Center.md)
- Windows chooses the fastest connection by default if you have multiple simultaneous connections e.g. wired, wireless, WWAN

#### Configuring IP address

- in case DHCP server is not available, set up an alternate connection in Network and Sharing Center > Change adapter settings
- from there, right click ethernet > Properties > select IPv4 > Properties 
- you'll see that an IP address is obtained automatically, you can also input your own IP address
- in the Alternate Configuration tab you'll see the private IP is automatic (APIPA)
- this is where you can again manually input your own IP, subnet mask, default gateway, and other IPv4 config details