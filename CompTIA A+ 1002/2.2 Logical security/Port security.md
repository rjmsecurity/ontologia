> 2.2 Explain logical security concepts. 

# Port security

- how will you prevent unauthorized users from connecting to a switch interface? 
- there are switch ports in the conference room, at your desk, inside the data center and wiring closets

- if somebody unplugs from a switch port and plugs in their own device, the port is disabled and/or you can receive an alert
- the source MAC (Media Access Control) address is used to determine if the device connecting to the port is authorized, even if forwarded from elsewhere

- the network admin can configure the switch with unique rules for each port
- some ports should have an unchanging MAC address, others don't need to 

- configure a maximum number of source MAC addresses on an interface
- e.g. only five MAC addresses communicating through a particular port
- the switch watches the MAC addresses coming through 
- as soon as the sixth address somes through, port security activates
- again, port security is configured by the network admin but the default is to disable the interface; you can have an alert