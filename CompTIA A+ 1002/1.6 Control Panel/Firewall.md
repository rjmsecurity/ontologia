> 1.5 Given a scenario, use Microsoft operating system features and tools. 
> 1.6 Given a scenario, use Microsoft Windows Control Panel utilities.
> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Windows Firewall
(part of the *administrative* tools category)

#### Intro
- Windows Firewall is *stateful* – it understands and remembers the state of traffic that flows through it
- if traffic is outbound, it knows to allow that same traffic flow inbound
- likewise if someone tried to send traffic inbound without there being an existing state, the firewall drops the packets
- Windows 10 renamed it from Windows Firewall to Windows *Defender* Firewall
- your firewall should always be on but sometimes you need to troubleshoot 
- Firewall has *public* and *private* network profiles if you want different settings for private networks vs. guest/public networks (e.g. coffee shop)

#### Features
- in the sidebar, *Allow an app or feature* lets you enable or disable connecting your apps to private and/or public networks
- it's a basic restriction if you want to have either any kind of inbound and outbound traffic or none at all
- or allow other people on your private network to access shares but block all connections in the public network profile  
- *Turn Windows Defender Firewall on or off* is fairly straightforward (the 🛡️ icon means you need elevated permissions)
- *Change notification settings* lets you disable getting that popup notification when Firewall is blocking a new app 
- again here you can have different settings for the private vs. public network profile
- also here you have a checkbox to block all incoming connections even to allowed apps 
- *Advanced settings* has more detailed control:
	- scope – inbound vs. outbound rules
	- connection security rules – encryption by sending packets through IPsec tunnels
	- granular rules – program, port, predefined services, custom variables
	- custom variables – program, port, protocol, scope of rule, action, profile
- in my Windows the public networks section says *Incoming connections: Block all connections to apps that are not on the list of allowed apps* 
