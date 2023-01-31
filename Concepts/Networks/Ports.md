# Well-known ports 

TCP/UDP | Port | Service | Description
-- | - | - | -
TCP | 20 | FTP | File Transfer Protocol, active mode data
TCP | 21 | FTP | File Transfer Protocol, control
TCP | 22 | SSH | Secure Shell
TCP | 23 | Telnet | Teletype (or telecommunications) network
TCP | 25 | SMTP | Simple Mail Transfer Protocol
UDP | 53 | DNS | Domain Name System
UDP | 67 | DHCP | Dynamic Host Configuration Protocol
UDP | 68 | DHCP | Dynamic Host Configuration Protocol
TCP | 80 | HTTP | Hypertext Transfer Protocol
TCP | 110 | POP3 | Post Office Protocol 3
UDP | 137 | SMB | NetBIOS (or NetBT) name services (nbname)
UDP | 138 | SMB | NetBIOS datagram service (nbdatagram); UDP version
TCP | 139 | SMB | NetBIOS session service (nbsession); TCP version
TCP | 143 | IMAP | Internet Mail Access Protocol (v4)
UDP | 161 | SNMP | Simple Network Management Protocol, queries
UDP | 162 | SNMP | Simple Network Management Protocol, traps
TCP | 389 | LDAP | Lightweight Directory Access Protocol
TCP | 427 | SLP | Service Location Protocol
UDP | 427 | SLP | Service Location Protocol
TCP | 443 | HTTPS | Hypertext Transfer Protocol Secure
TCP | 445 | SMB | Server Message Block (aka Common Internet File System, or CIFS)
TCP | 548 | AFP | Apple Filing Protocol
TCP | 587 | SMTP | SMTP with authentication
TCP | 993 | IMAPS | IMAP over SSL/TLS
TCP | 995 | POP3S | POP3 over SSL/TLS
TCP | 3389 | RDP | Remote Desktop Protocol

Messer writes "tcp" or "udp" and the port number together, e.g., *tcp/20*

**Introduced in CompTIA A+ 1101**

- **tcp/20, tcp/21 – File Transfer Protocol (FTP)** ⟹ transfer files between systems
	- tcp/20 is for data transfers (**active mode data**)
	- tcp/21 is to control the data transfers (**control**)
	- authentication via username and password
	- some systems allow generic/anonymous login with any or no password
	- full-featured file management functionality: list files, add, delete, rename, etc.
- **tcp/22 – Secure Shell (SSH) ⟹** connect to a remote device through a command line front end
	- we see plain text on our screen/it looks and acts the same as Telnet, but any communication sent over the network is encrypted
- **tcp/23 – Telnet ⟹** like SSH, a text-based front end to connect to remote console 
	- unlike SSH, communication is **in-the-clear** (unencrypted)
	- vulnerable to MITM attack
	- also I remember a THM lab going through logs on a system and finding Telnet commands, so you were able to see the login credentials, vs. SSH logs which were jumbled text
	- we say that *Telnet is not suited for production systems*
- **tcp/25 – Simple Mail Transfer Protocol (SMTP) ⟹** for sending emails (from email client to server) and for server-to-server email transfer 
- **udp/53 – Domain Name System (DNS) ⟹** resolves an IP address from a FQDN (fully qualified domain name) so that your system can communicate with the webserver (of YouTube or whatever website)
	- these are very critical resources because we cannot memorize IP addresses
	- also server IP addresses often change without notice
	- usually multiple DNS servers are in production
- **udp/67, udp/68 – Dynamic Host Configuration Protocol (DHCP) ⟹** automatic configuration of IP address, subnet mask, etc.
	- e.g. using mobile device on Wi-Fi network of a coffee shop and automatically receiving an IP address that you can use on that network
	- requires a DHCP server to assign these IP addresses, commonly built into SOHO routers and WAPs
		- dynamic/pooled — server has large **pool** of IP addresses that can be assigned to devices
		- assigned in real time: when you start up your computer, it queries the DHCP server, and the server assigns your device all of the IP configuration details
	- uses a **leasing** system to assign IP addresses, so you are only using IP address for certain amount of time; after lease expires and you are no longer on the network, that IP address goes back into the pool for somebody else to use
		- tl;dr each system is given a lease and must renew at set intervals
	- network admins can configure DHCP servers to always assign the same IP address to certain devices
		- routers, firewalls, switches, and other infrastructure devices
		- known as configuring **DHCP reservations** 
		- so those devices always receive the same IP addresses when they boot up
		- and if you need to make any IP configuration changes on those devices, you don't have to go to those devices, simply make them on the DHCP server, and the next time that device requests a new IP address it will receive the new configuration
		- IP addresses are assigned by MAC address on the DHCP server
- **tcp/80 – Hypertext Transfer Protocol (HTTP) ⟹** in-the-clear communication between browsers and web servers 
- **tcp/110 – Post Office Protocol 3 (POP3) ⟹** receive emails from an email server on an email client
	- authenticate and transfer
	- was not built for multiple clients which you probably have (e.g. phone, laptop)
- **tcp/143 – Internet Mail Access Protocol (IMAP) ⟹** downloading email inbox to multiple clients and management of that inbox from those multiple clients
	- IMAP4, Internet Mail Access Protocol v4
- **udp/161, udp/162 – Simple Network Management Protocol (SNMP) ⟹** for a network management device to query infrastructure devices for performance metrics
	- udp/161 for the **queries**
	- can configure the infrastructure devices to monitor for certain metrics and, if any of the metrics are exceeded, to send an alert to the management station
	- these alerts are called **traps**
	- udp/162 for traps
	- network admins are very familiar with SNMP
	- if you're configuring SNMP on a device, it will ask if you are using v1, v2, or v3
	- v1, the original, sent structured tables across the network in-the-clear
	- v2 had data type enhancements and allowed for bulk transfers of information
	- v3 introduced encryption, integrity, and authentication; a secure standard
	- [see Messer image at 10:00](https://youtu.be/dh8h-4u7Wak?t=600)
- **tcp/389 – Lightweight Directory Access Protocol (LDAP) ⟹** directories are used extensively on modern networks and LDAP is used to query these directories
	- store and retrieve information in a network directory
	- many implementations of LDAP and Microsoft Active Directory (AD) is one of the most popular, allowing you to query an AD server using the LDAP protocol
	- [see Messer image at 11:00](https://youtu.be/dh8h-4u7Wak?t=660)
- **tcp/443 – Hypertext Transfer Protocol Secure (HTTPS) ⟹** encrypted communication between web servers and clients
- **tcp/445 – Server Message Block (SMB)/Common Internet File System (CIFS) ⟹** Windows's own method of transferring files and info between Windows devices
	- SMB is also referred to as CIFS
	- file sharing (transferring files between devices) and printer sharing (sending print jobs to printers)
	- older Windows machines use Network Basic Input/Output System (NetBIOS)/**NetBIOS over TCP/IP** (NetBT) 
		- **udp/137 - NetBIOS name services (nbname)** 
			- so that NetBIOS can find devices on your network by their names
		- **tcp/139 - NetBIOS session service (nbsession)**
			- to set up a session and transfer data between devices
	- modern Windows devices communicate directly using TCP/IP (NetBIOS-less)
		- direct SMB connection over tcp/445
- **tcp/3389 – Remote Desktop Protocol (RDP) ⟹** remote access to someone's desktop; connecting to or receiving a remote desktop session
	- used by people who work in support roles or on a help desk
	- standard protocol used by Windows
	- Remote Desktop Services, available on many Windows versions; you probably have it built-in today
	- can be used to control entire system or just a single application from the server
	- servers run RDP almost exclusively on Windows, but there are clients that you can run on almost any OS—macOS, Linux, Unix, Android, iOS—to connect to a Windows device using RDP

**Introduced in CompTIA Network+**

