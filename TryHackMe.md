# TryHackMe

- [Tools](Concepts/Security/Tools.md)
- [Terms](Concepts/Security/Terms.md)

**Notes**
- it's `root` on Apple, Linux, and Android systems; `administrator` on MS Windows systems
- https://tryhackme.com/room/dnsindetail I think task 3 completes my knowledge of DNS records
- https://tryhackme.com/room/contentdiscovery for some OSINT methods
- `Content-Type: application/x-www-form-urlencoded` is a MUST when tinkering with requests and changing from GET to POST
- https://tryhackme.com/room/ssrfqi awesome ways to remediate ssrf
- https://tryhackme.com/room/sqlinjectionlm and https://portswigger.net/web-security/sql-injection (which has a good link to https://portswigger.net/web-security/sql-injection/cheat-sheet) for SQLi
- fuzzing (discovery) and bruteforcing (authentication) tools: burp intruder, Wfuzz, Ffuf
- "As we have a list of known usernames, each associated with a password, we can avoid a straight bruteforce and instead use a credential stuffing attack (pitchfork attack on burp intruder)." ... "Well done, you have successfully bruteforced the support login page with a credential stuffing attack!"
- user's ssh key in linux is probably located at `/home/<username>/.ssh/id_rsa`
- `curl -X POST -F "submit:<value>" -F "<file-parameter>:@<path-to-file>" <site>`
- ping = icmp echo
- interesting so the same reason that VPNs are useful in public wifi, because they encrypt traffic between the devices on the VPN which are themselves also part of different networks (e.g. yours is part of a coffee shop network), VPNs are useful for companies with multiple offices. so i guess other employees can't sniff your connection to another office of your company. the network you're on can't see what's happening in your vpn tunnel https://tryhackme.com/room/extendingyournetwork go to task 4 on vpn basics
- https://tryhackme.com/room/extendingyournetwork this deserves its own bullet point to, very important room you need to practice to really understand routing and switches and tcp 
- https://tryhackme.com/room/linuxfundamentalspart3
- https://tryhackme.com/room/windowsfundamentals2x0x relevant to the A+ along with the previous and following rooms on Windows (and Linux too but mainly Windows since it's the predominant dominant dominating dominator domination)
- Ohhhh CIDR notation is this: 192.x.x.x is 192.0.0.0/8, 192.168.x.x is 192.168.0.0/16, 192.168.1.x is 192.168.1.0/24... I wonder if there's a /32 or if that makes no sense. I thought it was right to left and that's why I failed to learn CIDR, but it's left to right. /24 doesn't refer to how many bits are free to change but how many are set in stone. /8 means the first 8 bits are set in stone, /16 means the first 16 bits are set in stone...
- So you hear about computers on a network being the print server... do they do it through SMB? Because I just learned that SMB is used to share files, printers, and other things... I remember learning in the A+ how to set up a print server through some Windows utility, but maybe that utility underneath uses SMB? 
- Does AD use SMB? Since SMB can be used to read and write files... 