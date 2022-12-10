# CompTIA A+ Core 2 (220-1002)

These objectives are copied from [CompTIA's objectives PDF](https://www.comptia.jp/pdf/comptia-a-220-1002-exam-objectives.pdf). Read more [about the A+](CompTIA%20A+%201000%20series.md) or see what [resources I used](Resources.md).

## 1.0 Operating Systems

### 1.1 Compare and contrast common operating system types and their purposes. 

- [Bit widths](Concepts/Systems/Bit%20widths.md)
	- RAM limitations 
	- Software compatibility 

- Workstation operating systems 
	- Microsoft Windows ==> most prevalent, most targeted
	- Apple Macintosh OS ==> less vulnerable, hardware is expensive
	- Linux ==> open source, under nobody's authority, helpful community

- Cell phone/tablet operating systems 
	- Microsoft Windows ==> (Windows Mobile) now deprecated with tablets today running full-blown Windows
	- Android ==> based on Linux, standards are developed by the Open Handset Alliance, apps are developed with the Android SDK on any workstation
	- iOS ==> closed source, apps are developed with the iOS SDK on macOS and must be approved
	- Chrome OS ==> many manufacturers, also based on the Linux kernel, apps are web-based, good internet recommended, also it's more of a workstation OS

- Vendor-specific limitations 
	- End-of-life ==> EOL policies and philosophies vary based on expectations about how often users will upgrade their device
	- Update limitations ==> iOS, Android, and Windows prompt you for updates while Chrome OS is automatic (*rolling release* update method)

- Compatibility concerns between operating systems ==> web-based is the most compatible

### 1.2 Compare and contrast features of Microsoft Windows versions.

- [Windows 7](Concepts/Systems/Windows%207.md) 
- [Windows 8.x](Concepts/Systems/Windows%208.x.md) 
- [Windows 8.x](Concepts/Systems/Windows%208.x.md) 
- [Windows 10](Concepts/Systems/Windows%2010.md) 
- [Hardware requirements](Concepts/Systems/Hardware%20requirements.md)
- Corporate vs. personal needs ==> [Corporate vs personal needs](Concepts/Business/Corporate%20vs%20personal%20needs.md)
	- Domain access 
	- BitLocker 
	- Media center 
	- BranchCache 
	- EFS 
- Desktop styles/user interface

### 1.3 Summarize general OS installation considerations and upgrade methods. 

- [Boot methods](Concepts/Systems/Boot%20methods.md)
	- Optical disc (CD-ROM, DVD, Blu-ray) 
	- External drive/flash drive (USB/eSATA) 
	- Network boot (PXE) 
	- Internal fixed disk (HDD/SSD) 
	- Internal hard drive (partition) 

- [Types of installations](Concepts/Systems/Types%20of%20installations.md)
	- Unattended installation 
	- In-place upgrade 
	- Clean install 
	- Repair installation 
	- Multiboot 
	- Remote network installation 
	- Image deployment 
	- Recovery partition 
	- Refresh/restore 

- [Partitioning](Concepts/Systems/Partitioning.md)
	- Dynamic 
	- Basic 
	- Primary 
	- Extended 
	- Logical 
	- GPT 

- File system types/formatting ==> [Formatting](Concepts/Systems/Formatting.md)
	- ExFAT 
	- FAT32 
	- NTFS 
	- CDFS 
	- NFS 
	- ext3, ext4 
	- HFS 
	- Swap partition 
	- Quick format vs. full format 

- Load alternate third-party drivers when necessary ==> [More on installing](Concepts/Systems/More%20on%20installing.md)
- Workgroup vs. Domain setup ==> if you're setting up for a Domain then you need the proper credentials to connect to that network
- Time/date/region/language settings 
- Driver installation, software, and Windows updates ==> perform an update after install to make sure you have the latest security patches
- Factory recovery partition ==> [Partitioning](Concepts/Systems/Partitioning.md)
- Properly formatted boot drive with the correct partitions/format 
- Prerequisites/hardware compatibility ==> use Windows 10 Upgrade Checker to ensure the hardware is compatible and you meet the minimum OS requirements 
- Application compatibility 
- OS compatibility/upgrade path ==> you can't upgrade from 32-bit to 64-bit or vice versa, you must migrate

### 1.4 Given a scenario, use appropriate Microsoft command line tools. 

- Navigation 
	- `dir` is the Windows `ls`
	- `cd` Windows isn't case sensitive so `cd \users` or `cd \Users`
	- `..` move up (or if Seinfeld, move down)
- `cls` is the Windows `clear`
- `ipconfig` ==> [Commands intro](Concepts/Systems/Commands%20intro.md)
- `ping` ==> [ping and tracert](Concepts/Networks/ping%20and%20tracert.md)
- `tracert` ==> [ping and tracert](Concepts/Networks/ping%20and%20tracert.md)
- `netstat` ==> [netstat and nslookup](Concepts/Networks/netstat%20and%20nslookup.md)
- `nslookup` ==> [netstat and nslookup](Concepts/Networks/netstat%20and%20nslookup.md)
- `shutdown` ==> [108. shutdown](./108.%20shutdown.md) 
- [dism](Concepts/Systems/dism.md)
- `sfc` ==> [sfc and chkdsk](Concepts/Systems/sfc%20and%20chkdsk.md)
- `chkdsk` ==> [sfc and chkdsk](Concepts/Systems/sfc%20and%20chkdsk.md)
- `diskpart` ==> [format and diskpart](Concepts/Systems/format%20and%20diskpart.md)
- `taskkill` ==> [Commands intro](Concepts/Systems/Commands%20intro.md)
- `gpupdate` ==> [gpupdate and gpresult](Concepts/Networks/gpupdate%20and%20gpresult.md)
- `gpresult` ==> [gpupdate and gpresult](Concepts/Networks/gpupdate%20and%20gpresult.md)
- `format` ==> [format and diskpart](Concepts/Systems/format%20and%20diskpart.md)
- `copy` ==> [copy](Concepts/Systems/copy.md)
- `xcopy` ==> [copy](Concepts/Systems/copy.md)
- `robocopy` ==> [copy](Concepts/Systems/copy.md)
- `net use` ==> [net](Concepts/Networks/net.md)
- `net user` ==> [net](Concepts/Networks/net.md)
- `[command name] /?` or `help [command name]`
- Commands available with standard privileges vs. administrative privileges ==> [Commands intro](Concepts/Systems/Commands%20intro.md)

### 1.5 Given a scenario, use Microsoft operating system features and tools. 

- Administrative 
	- Computer Management ==> [mmc](Concepts/Systems/mmc.md)
	- Device Manager ==> [devmgmt.msc](Concepts/Systems/devmgmt.msc.md)
	- [Local Users and Groups](Concepts/Systems/Local%20Users%20and%20Groups.md) 
	- [Local Security Policy](Concepts/Security/Local%20Security%20Policy.md)
	- Performance Monitor ==> [perfmon](Concepts/Systems/perfmon.md)
	- Services ==> [services.msc](Concepts/Systems/services.msc.md)
	- System Configuration ==> [MSConfig](Concepts/Systems/MSConfig.md)
	- [Task Scheduler](Concepts/Systems/Task%20Scheduler.md)
	- [Component Services](Concepts/Systems/Component%20Services.md)
	- [Data Sources](Concepts/Systems/Data%20Sources.md)
	- [Print Management](Concepts/Systems/Print%20Management.md)
	- Windows Memory Diagnostics ==> [Memory Diagnostics](Concepts/Systems/Memory%20Diagnostics.md)
	- Windows Firewall ==> [Firewall](Concepts/Security/Firewall.md)
	- Advanced Security ==> [Firewall](Concepts/Security/Firewall.md)
	- [Event Viewer](Concepts/Systems/Event%20Viewer.md)
	- User Account Management

- [MSConfig](Concepts/Systems/MSConfig.md)
	- General 
	- Boot 
	- Services 
	- Startup 
	- Tools 

- [Task Manager](Concepts/Systems/Task%20Manager.md)
	- Applications 
	- Processes 
	- Performance 
	- Networking 
	- Users 

- [Disk Management](Concepts/Systems/Disk%20Management.md)
	- Drive status 
	- Mounting 
	- Initializing 
	- Extending partitions 
	- Splitting partitions 
	- Shrink partitions 
	- Assigning/changing drive letters 
	- Adding drives 
	- [Adding arrays](Concepts/Systems/Adding%20arrays.md)
	- [Storage spaces](Concepts/Cloud/Storage%20spaces.md)

- System utilities 
	- Regedit ==> [regedit](Concepts/Systems/regedit.md)
	- Command 
	- Services.msc ==> [services.msc](Concepts/Systems/services.msc.md)
	- MMC ==> [mmc](Concepts/Systems/mmc.md)
	- MSTSC ==> [mstsc](Concepts/Systems/mstsc.md)
	- Notepad ==> text editor where you can view and edit log files for example
	- Explorer ==> Windows Explorer renamed to File Explorer in Windows 10; change permissions, access network resources/modify files in a share...
	- Msinfo32 ==> [msinfo32](Concepts/Systems/msinfo32.md)
	- DxDiag ==> [dxdiag](Concepts/Systems/dxdiag.md)
	- Disk Defragmenter ==> [defrag](Concepts/Systems/defrag.md)
	- [System Restore](Concepts/Systems/System%20Restore.md)
	- [Windows Update](Concepts/Systems/Windows%20Update.md)

### 1.6 Given a scenario, use Microsoft Windows Control Panel utilities.

- [Internet Options](Concepts/Systems/Internet%20Options.md)
	- Connections 
	- Security 
	- General 
	- Privacy 
	- Programs 
	- Advanced 

- Display/Display Settings ==> [Display](Concepts/Systems/Display.md)
	- Resolution 
	- Color depth 
	- Refresh rate 

- [User Accounts](Concepts/Systems/User%20Accounts.md)

- [Folder Options](Concepts/Systems/Folder%20Options.md)
	- View hidden files 
	- Hide extensions 
	- General options 
	- View options 

- [System](Concepts/Systems/System.md)
	- Performance (virtual memory) 
	- Remote settings 
	- System protection 

- Windows Firewall ==> [Firewall](Concepts/Security/Firewall.md)

- [Power Options](Concepts/Systems/Power%20Options.md)
	- Hibernate 
	- Power plans 
	- Sleep/suspend 
	- Standby 

- [Credential Manager](Concepts/Security/Credential%20Manager.md)
- [Programs and features](Concepts/Systems/Programs%20and%20features.md)
- [HomeGroup](Concepts/Networks/HomeGroup.md)
- [Devices and Printers](Concepts/Systems/Devices%20and%20Printers.md)
- Sound ==> settings for output and input options, and you can configure the line levels for each individual device
- [Troubleshooting](Concepts/Systems/Troubleshooting.md)
- [Network and Sharing Center](Concepts/Networks/Network%20and%20Sharing%20Center.md)
- [Device Manager](Concepts/Systems/Device%20Manager.md)
- [BitLocker](Concepts/Security/BitLocker.md)
- [Sync Center](Concepts/Networks/Sync%20Center.md)

### 1.7 Summarize application installation and configuration concepts. 

- System requirements ==> [App install requirements](Concepts/Systems/App%20install%20requirements.md)
	- Drive space 
	- RAM 

- OS requirements ==> [App install requirements](Concepts/Systems/App%20install%20requirements.md)
	- Compatibility 

- Methods of installation and deployment ==> [Install methods](Concepts/Systems/Install%20methods.md)
	- Local (CD/USB) 
	- Network-based 

- [Local user permissions](Concepts/Security/Local%20user%20permissions.md)
	- Folder/file access for installation 

- [Security considerations](Concepts/Security/Security%20considerations.md)
	- Impact to device 
	- Impact to network

### 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

- [HomeGroup](Concepts/Networks/HomeGroup.md) vs. [WorkGroup](Concepts/Networks/WorkGroup.md)
- Domain setup ==> [Domain](Concepts/Networks/Domain.md)
- Network shares/administrative shares/mapping drives ==> [Network shares](Concepts/Networks/Network%20shares.md) and [Mapping drives](Concepts/Networks/Mapping%20drives.md)
- Printer sharing vs. network printer mapping ==> [Printer sharing](Concepts/Networks/Printer%20sharing.md)

- Establish networking connections ==> [Network and Sharing Center](Concepts/Networks/Network%20and%20Sharing%20Center.md)
	- VPN ==> [VPN](Concepts/Networks/VPN.md)
	- Dial-ups ==> [Dial-ups](Concepts/Networks/Dial-ups.md)
	- Wireless ==> [Wireless](Concepts/Networks/Wireless.md)
	- Wired ==> [Wired](Concepts/Networks/Wired.md)
	- WWAN (Cellular) ==> [WWAN](Concepts/Networks/WWAN.md)

- Proxy settings ==> [Proxy settings](Concepts/Networks/Proxy%20settings.md)
- Remote Desktop Connection ==> [Remote Desktop Connection](Concepts/Networks/Remote%20Desktop%20Connection.md)
- Remote Assistance ==> [Remote Assistance](Concepts/Networks/Remote%20Assistance.md)
- Home vs. Work vs. Public network settings ==> [Home vs. Work vs. Public](Concepts/Networks/Home%20vs.%20Work%20vs.%20Public.md)
- Firewall settings ==> [Firewall advanced](Concepts/Networks/Firewall%20advanced.md)
	- Exceptions 
	- Configuration 
	- Enabling/disabling Windows Firewall 

- Configuring an alternative IP address in Windows ==> [IP address](Concepts/Networks/IP%20address.md)
	- IP addressing 
	- Subnet mask 
	- DNS 
	- Gateway 

- Network card properties 
	- Half duplex/full duplex/auto ==> [Link speed and duplex](Concepts/Networks/Link%20speed%20and%20duplex.md)
	- Speed ==> [Link speed and duplex](Concepts/Networks/Link%20speed%20and%20duplex.md)
	- Wake-on-LAN ==> [Wake-on-LAN](Concepts/Networks/Wake-on-LAN.md)
	- QoS ==> [QoS](Concepts/Networks/QoS.md)
	- BIOS (on-board NIC) ==> [BIOS](Concepts/Networks/BIOS.md)

### 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

- Best practices 
	- Scheduled backups ==> [Time Machine](Concepts/Systems/Time%20Machine.md)
	- Scheduled disk maintenance ==> [Disk Utility](Concepts/Systems/Disk%20Utility.md) and [Disk maintenance](Concepts/Systems/Disk%20maintenance.md)
	- System updates/App Store ==> [App Store](Concepts/Systems/App%20Store.md) and [apt-get and yum](Concepts/Systems/apt-get%20and%20yum.md)
	- Patch management ==> [App Store](Concepts/Systems/App%20Store.md) and [apt-get and yum](Concepts/Systems/apt-get%20and%20yum.md)
	- Driver/firmware updates ==> [System Information](Concepts/Systems/System%20Information.md) and [apt-get and yum](Concepts/Systems/apt-get%20and%20yum.md)
	- Antivirus/Anti-malware updates ==> [Antivirus](Concepts/Security/Antivirus.md)
- Tools 
	- Backup/Time Machine ==> [Time Machine](Concepts/Systems/Time%20Machine.md)
	- Restore/Snapshot ==> [Time Machine](Concepts/Systems/Time%20Machine.md)
	- Image recovery ==> [Disk Utility](Concepts/Systems/Disk%20Utility.md)
	- Disk maintenance utilities ==> [Disk Utility](Concepts/Systems/Disk%20Utility.md)
	- Shell/Terminal ==> [Terminal](Concepts/Systems/Terminal.md)
	- [Screen sharing](Concepts/Systems/Screen%20sharing.md)
	- [Force Quit](Concepts/Systems/Force%20Quit.md)
- Features 
	- Multiple desktops/Mission Control ==> [Mission Control](Concepts/Systems/Mission%20Control.md)
	- [Keychain](Concepts/Security/Keychain.md)
	- [Spotlight](Concepts/Systems/Spotlight.md)
	- [iCloud](Concepts/Cloud/iCloud.md)
	- Gestures ==> [Mission Control](Concepts/Systems/Mission%20Control.md)
	- [Finder](Concepts/Systems/Finder.md)
	- [Remote Disc](Concepts/Systems/Remote%20Disc.md)
	- [Dock](Concepts/Systems/Dock.md)
	- [Boot Camp](Concepts/Systems/Boot%20Camp.md)

- Basic Linux commands 
	- ls ==> [Unix commands intro](Concepts/Systems/Unix%20commands%20intro.md)
	- grep ==> [Unix commands intro](Concepts/Systems/Unix%20commands%20intro.md)
	- cd ==> [Unix commands intro](Concepts/Systems/Unix%20commands%20intro.md)
	- [shutdown](Concepts/Systems/shutdown.md)
	- pwd vs. passwd ==> [Unix commands intro](Concepts/Systems/Unix%20commands%20intro.md) vs. [passwd](Concepts/Systems/passwd.md)
	- mv ==> [Files and folders](Concepts/Systems/Files%20and%20folders.md)
	- cp ==> [Files and folders](Concepts/Systems/Files%20and%20folders.md)
	- rm ==> [Files and folders](Concepts/Systems/Files%20and%20folders.md)
	- [chmod](Concepts/Systems/chmod.md)
	- [chown](Concepts/Systems/chown.md)
	- [iwconfig and ifconfig](Concepts/Networks/iwconfig%20and%20ifconfig.md)
	- [ps](Concepts/Systems/ps.md)
	- [su and sudo](Concepts/Systems/su%20and%20sudo.md)
	- [apt-get](Concepts/Systems/apt-get.md)
	- [vi](Concepts/Systems/vi.md)
	- [dd](Concepts/Systems/dd.md)
	- [kill](Concepts/Systems/kill.md)

## 2.0 Security

### 2.1 Summarize the importance of physical security measures.

- Access control vestibule ==> [Entrance security](Concepts/Security/Entrance%20security.md)
- Badge reader ==> [Entrance security](Concepts/Security/Entrance%20security.md)
- Smart card ==> [Tokens](Concepts/Security/Tokens.md)
- Security guard ==> [Entrance security](Concepts/Security/Entrance%20security.md)
- Door lock ==> [Door locks](Concepts/Security/Door%20locks.md)
- Biometric locks ==> [Door locks](Concepts/Security/Door%20locks.md)
- Hardware tokens ==> [Tokens](Concepts/Security/Tokens.md)
- Cable locks ==> [Other physical measures](Concepts/Security/Other%20physical%20measures.md)
- Server locks ==> [Other physical measures](Concepts/Security/Other%20physical%20measures.md)
- USB locks ==> [Other physical measures](Concepts/Security/Other%20physical%20measures.md)
- Privacy screen ==> [Other physical measures](Concepts/Security/Other%20physical%20measures.md)
- Key fobs ==> [Door locks](Concepts/Security/Door%20locks.md)
- Entry control roster ==> [Entrance security](Concepts/Security/Entrance%20security.md)

### 2.2 Explain logical security concepts. 

- [Active Directory](Concepts/Security/Active%20Directory.md)
	- Login script 
	- Domain 
	- Group Policy/Updates 
	- Organizational Units 
	- Home Folder 
	- Folder redirection 

- Software tokens 
- MDM policies ==> [MDM](Concepts/Security/MDM.md)
- [Port security](Concepts/Security/Port%20security.md)
- MAC address filtering ==> [MAC filtering](Concepts/Security/MAC%20filtering.md)
- [Certificates](Concepts/Security/Certificates.md)
- Antivirus/Anti-malware ==> [Security admin](Concepts/Security/Security%20admin.md)
- Firewalls
- User authentication/strong passwords 
- Multifactor authentication 
- Directory permissions 
- VPN 
- DLP 
- Access control lists 
- Smart card 
- Email filtering 
- Trusted/untrusted software sources 
- Principle of least privilege

### 2.3 Compare and contrast wireless security protocols and authentication methods. 

- Protocols and encryption 
	- WEP 
	- WPA 
	- WPA2 
	- TKIP 
	- AES 
- Authentication 
	- Single-factor 
	- Multifactor 
	- RADIUS 
	- TACACS

### 2.4 Given a scenario, detect, remove, and prevent malware using appropriate tools and methods. 

- Malware 
	- Ransomware 
	- Trojan 
	- Keylogger 
	- Rootkit 
	- Virus 
	- Botnet 
	- Worm 
	- Spyware 
- Tools and methods 
	- Antivirus 
	- Anti-malware 
	- Recovery console 
	- Backup/restore 
	- End user education 
	- Software firewalls 
	- DNS configuration

### 2.5 Compare and contrast social engineering, threats, and vulnerabilities. 

- Social engineering 
	- Phishing 
	- Spear phishing 
	- Impersonation 
	- Shoulder surfing 
	- Tailgating 
	- Dumpster diving 
- DDoS 
- DoS 
- Zero-day 
- On-path attack (previously known as man-in-the-middle attack) 
- Brute force 
- Dictionary 
- Rainbow table 
- Spoofing 
- Non-compliant systems 
- Zombie

### 2.6 Compare and contrast the differences of basic Microsoft Windows OS security settings. 

- User and groups 
	- Administrator 
	- Power user 
	- Guest 
	- Standard user 
- NTFS vs. share permissions 
	- Allow vs. deny 
	- Moving vs. copying folders and files 
	- File attributes 
- Shared files and folders 
	- Administrative shares vs. local shares 
	- Permission propagation 
	- Inheritance 
- System files and folders 
- User authentication 
	- Single sign-on 
- Run as administrator vs. standard user 
- BitLocker 
- BitLocker To Go 
- EFS

### 2.7 Given a scenario, implement security best practices to secure a workstation.

- Password best practices 
	- Setting strong passwords 
	- Password expiration 
	- Screensaver required password 
	- BIOS/UEFI passwords 
	- Requiring passwords 
- Account management 
	- Restricting user permissions 
	- Logon time restrictions 
	- Disabling guest account 
	- Failed attempts lockout 
	- Timeout/screen lock 
	- Change default admin user account/password 
	- Basic Active Directory functions 
		- Account creation 
		- Account deletion 
		- Password reset/unlock account 
		- Disable account 
- Disable autorun 
- Data encryption 
- Patch/update management

### 2.8 Given a scenario, implement methods for securing mobile devices. 

- Screen locks 
	- Fingerprint lock 
	- Face lock 
	- Swipe lock
	- Passcode lock 
- Remote wipes 
- Locator applications 
- Remote backup applications 
- Failed login attempts restrictions 
- Antivirus/Anti-malware 
- Patching/OS updates 
- Biometric authentication 
- Full device encryption 
- Multifactor authentication 
- Authenticator applications 
- Trusted sources vs. untrusted sources 
- Firewalls 
- Policies and procedures 
	- BYOD vs. corporate-owned 
	- Profile security requirements

### 2.9 Given a scenario, implement appropriate data destruction and disposal methods. 

- Physical destruction 
	- Shredder 
	- Drill/hammer 
	- Electromagnetic (Degaussing) 
	- Incineration 
	- Certificate of destruction 
- Recycling or repurposing best practices 
	- Low-level format vs. standard format 
	- Overwrite 
	- Drive wipe

### 2.10 Given a scenario, configure security on SOHO wireless and wired networks. 

- Wireless-specific 
	- Changing default SSID 
	- Setting encryption 
	- Disabling SSID broadcast 
	- Antenna and access point placement 
	- Radio power levels 
	- WPS 
- Change default usernames and passwords 
- Enable MAC filtering 
- Assign static IP addresses 
- Firewall settings 
- Port forwarding/mapping 
- Disabling ports 
- Content filtering/parental controls 
- Update firmware 
- Physical security

## 3.0 Software Troubleshooting

### 3.1 Given a scenario, troubleshoot Microsoft Windows OS problems. 

- Common symptoms 
	- Slow performance 
	- Limited connectivity 
	- Failure to boot 
	- No OS found 
	- Application crashes 
	- Blue screens 
	- Blank screens 
	- Printing issues 
	- Services fail to start 
	- Slow bootup 
	- Slow profile load 
- Common solutions 
	- Defragment the hard drive 
	- Reboot 
	- Kill tasks 
	- Restart services 
	- Update network settings 
	- Reimage/reload OS 
	- Roll back updates 
	- Roll back devices drivers 
	- Apply updates 
	- Repair application 
	- Update boot order 
	- Disable Windows services/applications 
	- Disable application startup 
	- Safe boot 
	- Rebuild Windows profiles

### 3.2 Given a scenario, troubleshoot and resolve PC security issues. 

- Common symptoms 
	- Pop-ups 
	- Browser redirection 
	- Security alerts 
	- Slow performance 
	- Internet connectivity issues 
	- PC/OS lockup 
	- Application crash 
	- OS updates failures 
	- Rogue antivirus 
	- Spam 
	- Renamed system files 
	- Disappearing files 
	- File permission changes 
	- Hijacked email 
		- Responses from users regarding email 
		- Automated replies from unknown sent email 
	- Access denied 
	- Invalid certificate (trusted root CA) 
	- System/application log errors

### 3.3 Given a scenario, use best practice procedures for malware removal. 

1. Identify and research malware symptoms. 
2. Quarantine the infected systems. 
3. Disable System Restore (in Windows). 
4. Remediate the infected systems.
	1. Update the anti-malware software. 
	2. Scan and use removal techniques (safe mode, pre-installation environment).
5. Schedule scans and run updates. 
6. Enable System Restore and create a restore point (in Windows). 
7. Educate the end user.

### 3.4 Given a scenario, troubleshoot mobile OS and application issues. 

- Common symptoms 
	- Dim display 
	- Intermittent wireless 
	- No wireless connectivity 
	- No Bluetooth connectivity 
	- Cannot broadcast to external monitor 
	- Touchscreen non-responsive 
	- Apps not loading 
	- Slow performance 
	- Unable to decrypt email 
	- Extremely short battery life 
	- Overheating 
	- Frozen system 
	- No sound from speakers 
	- Inaccurate touch screen response 
	- System lockout 
	- App log errors

### 3.5 Given a scenario, troubleshoot mobile OS and application security issues. 

- Common symptoms 
	- Signal drop/weak signal 
	- Power drain 
	- Slow data speeds 
	- Unintended WiFi connection 
	- Unintended Bluetooth pairing 
	- Leaked personal files/data 
	- Data transmission over limit 
	- Unauthorized account access 
	- Unauthorized location tracking 
	- Unauthorized camera/microphone activation 
	- High resource utilization

## 4.0 Operational Procedures

### 4.1 Compare and contrast best practices associated with types of documentation. 

- Network topology diagrams 
- Knowledge base/articles 
- Incident documentation 
- Regulatory and compliance policy 
- Acceptable use policy 
- Password policy 
- Inventory management 
	- Asset tags 
	- Barcodes

### 4.2 Given a scenario, implement basic change management best practices.

- Documented business processes 
- Purpose of the change 
- Scope the change 
- Risk analysis 
- Plan for change 
- End-user acceptance 
- Change board 
	- Approvals 
- Backout plan 
- Document changes

### 4.3 Given a scenario, implement basic disaster prevention and recovery methods. 

- Backup and recovery 
	- Image level 
	- File level 
	- Critical applications 
- Backup testing 
- UPS 
- Surge protector 
- Cloud storage vs. local storage backups 
- Account recovery options

### 4.4 Explain common safety procedures. 

- Equipment grounding 
- Proper component handling and storage 
	- Antistatic bags 
	- ESD straps 
	- ESD mats 
	- Self-grounding 
- Toxic waste handling 
	- Batteries 
	- Toner 
	- CRT 
	- Cell phones 
	- Tablets 
- Personal safety 
	- Disconnect power before repairing PC 
	- Remove jewelry 
	- Lifting techniques 
	- Weight limitations 
	- Electrical fire safety 
	- Cable management 
	- Safety goggles 
	- Air filter mask 
- Compliance with government regulations

### 4.5 Explain environmental impacts and appropriate controls. 

- MSDS documentation for handling and disposal 
- Temperature, humidity level awareness, and proper ventilation 
- Power surges, under-voltage events, and power loss 
	- Battery backup 
	- Surge suppressor 
- Protection from airborne particles 
	- Enclosures 
	- Air filters/mask 
- Dust and debris 
	- Compressed air 
	- Vacuums 
- Compliance to government regulations

### 4.6 Explain the processes for addressing prohibited content/activity, and privacy, licensing, and policy concepts. 

- Incident response 
	- First response 
		- Identify 
		- Report through proper channels 
		- Data/device preservation 
	- Use of documentation/documentation changes 
	- Chain of custody 
		- Tracking of evidence/ documenting process 
- Licensing/DRM/EULA 
	- Open-source vs. commercial license 
	- Personal license vs. enterprise licenses 
- Regulated data 
	- PII 
	- PCI 
	- GDPR 
	- PHI 
- Follow all policies and security best practices

### 4.7 Given a scenario, use proper communication techniques and professionalism. 

- Use proper language and avoid jargon, acronyms, and slang, when applicable 
- Maintain a positive attitude/ project confidence 
- Actively listen (taking notes) and avoid interrupting the customer 
- Be culturally sensitive 
	- Use appropriate professional titles, when applicable 
- Be on time (if late, contact the customer) 
- Avoid distractions 
	- Personal calls 
	- Texting/social media sites 
	- Talking to coworkers while interacting with customers 
	- Personal interruptions 
- Dealing with difficult customers or situations 
	- Do not argue with customers and/or be defensive 
	- Avoid dismissing customer problems 
	- Avoid being judgmental 
	- Clarify customer statements (ask open-ended questions to narrow the scope of the problem, restate the issue, or question to verify understanding) 
	- Do not disclose experiences via social media outlets 
- Set and meet expectations/timeline and communicate status with the customer 
	- Offer different repair/replacement options, if applicable 
	- Provide proper documentation on the services provided 
	- Follow up with customer/user at a later date to verify satisfaction 
- Deal appropriately with customers’ confidential and private materials 
	- Located on a computer, desktop, printer, etc.

### 4.8 Identify the basics of scripting.

- Script file types 
	- .bat 
	- .ps1 
	- .vbs 
	- .sh 
	- .py 
	- .js 
- Environment variables 
- Comment syntax 
- Basic script constructs 
	- Basic loops 
	- Variables 
- Basic data types 
	- Integers 
	- Strings

### 4.9 Given a scenario, use remote access technologies.

- RDP
- Telnet
- SSH
- Third-party tools
	- Screen share feature
	- File share
- Security considerations of each access method