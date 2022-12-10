# QoS
(part of the *Network card properties* section)

- your traffic is a mix of VoIP, print jobs, file transfers, applications, video streaming
- if you want to prioritize VoIP then use QoS 
- DSCP (Differentiated Services Code Points) is a Windows feature that uses a type of QoS
- in the IP header are DSCP fields and they allow the network admin to assign different priorities to different types of traffic
- in IPv4 there is a ToS (Type of Service) field and in IPv6 it's the Traffic Class octet idk why we are learning this
- sysadmin assigns priorities on a workstation by workstation basis from Local Computer Policy
- or Group Policy if you're in a Domain
- from there go to Computer Configuration > Windows Settings > Policy-based QoS
- right click Policy-based QoS and *Create new policy* 
- Specify a DSCP value, throttle rate, application names 
- e.g. network admin told you a DSCP value of 2 is associated with web traffic so you name the policy *Web* and specify *2*
- specify all apps or a particular app e.g. notepad.exe
- assign source and destination IP addresses
- finally assign source and port numbers e.g. destination port 80 traffic is associated with this policy
- in other words, if notepad.exe is sending any outbound traffic to port 80 it'll be assigned a DSCP value of 2
- as this traffic goes out the network admin has a QoS device that prioritizes traffic based on these DSCP values

#aplus #core2 **1.8** *Given a scenario, configure Microsoft Windows networking on a client/desktop.*
