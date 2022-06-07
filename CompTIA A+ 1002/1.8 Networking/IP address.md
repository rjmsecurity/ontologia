> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Configuring IP address

- for some reason, the actual steps to configure your IP address are back in [Wired](Wired.md)
- Windows obtains an IP address automatically by default when you start up
- DHCP (Dynamic Host Configuration Protocol) is responsible for finding a DHCP server, obtaining and assigning an IP address to your computer
- at home there is usually one DHCP server that's integrated into your wireless router but at work you need redundancy so there are multiple servers

#### APIPA and the *Alternative configuration* tab

- if Windows cannot find the DHCP server and a static address has not been assigned, it creates an APIPA address (Automatic Private IP Addressing) 
- APIPA address is also known as a link-local address and is able to communicate locally, with other devices on the network, but no internet 
- you know you've been assigned an APIPA address if it's in the range 169.254.1.0 to 169.254.254.255
- you can set an alternative to the APIPA address when a DHCP server is unavailable by going to the *Alternative Configuration* tab

#### Static IP address and the *General* tab

- in some environments a network admin does not want to use DHCP or APIPA and manually assigns all IP address parameters
- this static IP address is set in the *General* tab of the IPv4 Properties dialog 
- if you turn off dynamic IP by turning on static IP then the Alternative Configuration tab will disappear
- the parameters the network admin needs to know include: the IP address itself which cannot match any other on the network
- a subnet mask, which identifies the particular IP subnet you're a member of
- a default gateway, or the device that allows communication outside of your local subnet
- DNS (Domain Name Services) IP address so that you can browse website domains instead of typing IP addresses
- the DHCP server may be configured to assign from a pool of available IP addresses or an IP address that is always assigned to you based on your MAC address
- every device has a loopback address, the default being 127.0.0.1, for when you want to reference your local computer by IP address