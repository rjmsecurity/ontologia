> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Domain

- in a WorkGroup, you're using one set of credentials for the accounting department printer, another set of credentials for the legal department documents...
- *Domain* lets you manage authentication from a centralized service and can scale from a small organization to thousands of computers
- you add users to a centralized domain called Active Directory Domain Services and authenticate those users to any resource/share on the network
- you can also manage any aspect of the OS and update or install applications from that one central database
- again, Control Panel > System

#### Domain setup 

- you cannot join a domain with Windows Home, must be at least Pro
- Control Panel > System > *Change settings* link to join a domain
- from there, the Computer Name tab is selected by default > *To use a wizard to join a domain or workgroup, click Network ID*
- go through the steps in the wizard – this computer *is* part of a business network, it *is* with a domain, then provide all the credentials your sysadmin gave you
- so check with the local administrator to get proper access to the domain if you don't have the username, password, computer name, etc. 