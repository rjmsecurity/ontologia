This is a copy of [objectives.md](objectives.md) but with my notes for each bullet point topic. 

# A+ 1001 Outline

## 1.0 Mobile Devices
### 1.1 Given a scenario, install and configure laptop hardware and components.
- Hardware/device replacement
	- Keyboard
	- Hard drive
		- SSD vs. hybrid vs. magnetic disk
		- 1.8in vs. 2.5in
	- Memory
	- Smart card reader
	- Optical drive
	- Wireless card/Bluetooth module
	- Cellular card
	- Video card
	- **Mini PCIe**
	- Screen
	- **DC jack**
	- Battery
	- Touchpad
	- Plastics/frames
	- Speaker
	- **System board**
	- CPU

### 1.2 Given a scenario, install components within the display of a laptop.
- Types 
	- LCD — backlit by CCFL or LED, either case an inverter is needed
	- OLED — doesn't need a backlight, but is expensive and not yet common on laptops
- WiFi antenna connector/placement 
- Webcam 
- Microphone 
- Inverter — takes low DC voltage from laptop and converts it to high AC voltage for backlight
- Digitizer/touchscreen — touch screens can be resistive or capacitative

### 1.3 Given a scenario, use appropriate laptop features.
- Special function keys 
	- Dual displays 
	- Wireless (on/off) 
	- Cellular (on/off) 
	- Volume settings 
	- Screen brightness 
	- Bluetooth (on/off) 
	- Keyboard backlight 
	- Touchpad (on/off) 
	- Screen orientation 
	- Media options (fast forward/rewind) 
	- GPS (on/off) 
	- Airplane mode 
- Docking station 
- **Port replicator** 
- Physical laptop lock and cable lock 
- Rotating/removable screens

### 1.4 Compare and contrast characteristics of various types of other mobile devices.
- Tablets 
- Smartphones 
- Wearable technology devices 
	- Smart watches 
	- Fitness monitors 
	- VR/AR headsets 
- E-readers 
- GPS

### 1.5 Given a scenario, connect and configure accessories and ports of other mobile devices.
- Connection types 
	- Wired 
		- **Micro-USB/Mini-USB**/USB-C 
		- Lightning 
		- Tethering 
		- Proprietary vendor-specific ports (communication/power) 
	- Wireless 
		- NFC 
		- Bluetooth 
		- **IR** 
		- Hotspot 
- Accessories 
	- Headsets 
	- Speakers 
	- Game pads 
	- Extra battery packs/battery chargers 
	- Protective covers/waterproofing 
	- Credit card readers 
	- Memory/MicroSD

### 1.6 Given a scenario, configure basic mobile device network connectivity and application support.
- Wireless/cellular data network (enable/disable) 
	- Hotspot 
	- Tethering 
	- Airplane mode 
- Bluetooth 
	- Enable Bluetooth 
	- Enable pairing 
	- Find a device for pairing 
	- Enter the appropriate pin code 
	- Test connectivity 
- Corporate and ISP email configuration 
	- POP3 
	- IMAP 
	- Port and SSL settings
	- **S/MIME** 
- Integrated commercial provider email configuration 
	- iCloud 
	- Google/Inbox 
	- Exchange Online 
	- Yahoo 
- **PRI** updates/PRL updates/**baseband** updates — prl is preferred roaming list and you should download it if you can't connect to carrier network outside of home, and pri is something something interface I think and it's just updates for something
- Radio firmware 
- IMEI vs. IMSI — **imsi identifies phone and network, imei identifies globally unique phone**
- VPN

### 1.7 Given a scenario, use methods to perform mobile device synchronization.
- Synchronization methods 
	- Synchronize to the cloud 
	- Synchronize to the desktop 
	- Synchronize to the automobile 
- Types of data to synchronize 
	- Contacts 
	- Applications 
	- Email 
	- Pictures 
	- Music 
	- Videos 
	- Calendar
	- Bookmarks 
	- Documents 
	- Location data 
	- Social media data 
	- E-books 
	- Passwords 
- Mutual authentication for multiple services (SSO) 
- Software requirements to install the application on the PC 
- Connection types to enable synchronization

## 2.0 Networking
### 2.1 Compare and contrast TCP and UDP ports, protocols, and their purposes.
- [ports.md](ports.md)
- TCP vs. UDP

### 2.2 Compare and contrast common networking hardware devices. 
- Routers
- Switches 
	- **Managed**
	- **Unmanaged**
- Access points
- **Cloud-based network controller** 
- Firewall
- Network interface card
- **Repeater**
- Hub
- **Cable/DSL modem**
- **Bridge**
- **Patch panel**
- Power over Ethernet (PoE)
	- **Injectors**
	- **Switch**
- Ethernet over Power

### 2.3 Given a scenario, install and configure a basic wired/wireless SOHO network.
- Router/switch functionality
- Access point settings 
- IP addressing
- NIC configuration
	- Wired
	- Wireless
- End-user device configuration
- IoT device configuration
	- Thermostat
	- Light switches
	- Security cameras
	- Door locks
	- Voice-enabled, smart speaker/digital assistant
- Cable/DSL modem configuration
- Firewall settings
	- Screened subnet (previously known as demilitarized zone)
	- Port forwarding
	- NAT
	- **UPnP**
	- Allow list/deny list
	- MAC filtering
- **QoS**
- Wireless settings
	- Encryption
	- Channels
	- QoS

### 2.4 Compare and contrast wireless networking protocols.
- **802.11(a, b, g, n, ac)**
- Frequencies
	- 2.4Ghz
	- 5Ghz
- Channels
	- **1-11**
- Bluetooth — aka PAN, range about 10m
- NFC — about 10cm range
- RFID
- Zigbee — this and Z-Wave are for internet of things
- Z-Wave
- 3G
- 4G
- 5G
- LTE

### 2.5 Summarize the properties and purposes of services provided by networked hosts.
- Server roles
	- Web server
	- File server
	- Print server
	- DHCP server
	- DNS server
	- **Proxy server**
	- Mail server
	- Authentication server
	- syslog
- Internet appliance
	- **UTM**
	- IDS
	- IPS
	- **End-point management server**
- Legacy/embedded systems

### 2.6 Explain common network configuration concepts. 
- IP addressing
	- Static
	- Dynamic
	- APIPA — address range is ***169.254***.0.1 to ***169.254***.255.254 but since the first and last 256 addresses are reserved it's ***169.254***.1.0 to ***169.254***.254.255
	- **Link local**
- DNS
- DHCP
	- Reservations
- IPv4 vs. IPv6
- **Subnet mask**
- **Gateway**
- VPN
- VLAN
- NAT

### 2.7 Compare and contrast Internet connection types, network types, and their features.
- **Internet connection types**
	- Cable — uses cable TV lines, up to 300 Mbps
	- DSL 
	- Dial-up
	- Fiber — SMF goes longer distances and uses laser so more expensive, MMF uses LED
	- Satellite
	- ISDN
	- Cellular
		- Tethering
		- Mobile hotspot
	- Line-of-sight wireless Internet service
- Network types
	- LAN
	- WAN
	- PAN
	- MAN
	- **WMN**

### 2.8 Given a scenario, use appropriate networking tools. 
- Crimper
- Cable stripper
- Multimeter
- Tone generator and probe
- **Cable tester**
- Loopback plug
- **Punchdown tool**
- WiFi analyzer

## 3.0 Hardware
### 3.1 Explain basic cable types, features, and their purposes.
- Network cables
	- Ethernet
		- Cat 5
		- Cat 5e
		- Cat 6
		- Plenum — counterpart to PVC which poisons when burned; plenum shielding is safe, more expensive, rated for plenum which refers to the air ducts above office rooms
		- Shielded twisted pair
		- Unshielded twisted pair
		- 568A/B — green and orange are switched
	- Fiber — fyi this isn't just for ethernet but some headphones have fiber connectors
	- Coaxial
	- Speed and transmission limitations
- Video cables
	- VGA
	- HDMI
	- Mini-HDMI
	- DisplayPort — has that notch on one corner
	- DVI (DVI-D/DVI-I)
- Multipurpose cables
	- Lightning
	- Thunderbolt — looks like USB-C ? lightning symbol
	- USB
	- USB-C
	- USB 2.0
	- USB 3.0
- Peripheral cables
	- Serial — 9 pin RS-232 connector
- **Hard drive cables**
	- SATA
	- IDE
	- SCSI
- Adapters
	- DVI to HDMI
	- USB to Ethernet
	- DVI to VGA

### 3.2 Identify common connector types.
- RJ-11 — RJ-11 has 6, RJ-45 has 8... I forgot of what, RJ-11 is like a thinner and taller RJ-45
- RJ-45 — network cable connections
- RS-232 — 9 pin, for serial ports
- BNC
- RG-59
- RG-6
- USB — (type A)
- Micro-USB
- Mini-USB
- USB-C
- DB-9 — exactly like RS-232... oh no i can't do this anymore
- Lightning
- SCSI
- eSATA
- **Molex** — voltages: 
- DisplayPort — has diagonal notch on one corner
- Mini DisplayPort — found on laptops, like a small fat rectangle
- HDMI — you know what it looks like
- mini-DIN (PS/2) — round (and old, but having a renaissance), keyboards and mice
- Parallel port (LPT port) — exclusively for printers 
- Serial port
- VGA — old, monitors

### 3.3 Given a scenario, install RAM types. 
- RAM types
	- SODIMM
	- DDR2
	- DDR3
	- DDR4
- Single channel
- Dual channel
- Triple channel
- Error correcting
- Parity vs. non-parity

### 3.4 Given a scenario, select, install and configure storage devices.
- Optical drives
	- CD-ROM/CD-RW
	- DVD-ROM/DVD-RW/DVD-RW DL
	- Blu-ray
	- BD-R
	- BD-RE
- Solid-state drives
	- M2 drives
	- NVME
	- SATA 2.5
- Magnetic hard drives
	- 5,400rpm
	- 7,200rpm
	- 10,000rpm
	- 15,000rpm
	- Sizes:
		- 2.5
		- 3.5
- Hybrid drives
- Flash
	- SD card
	- CompactFlash
	- Micro-SD card
	- Mini-SD card
	- xD
- Configurations
	- [RAID.md](RAID.md)
	- Hot swappable

### 3.5 Given a scenario, install and configure motherboards, CPUs, and add-on cards.
- Motherboard form factor
	- ATX
	- mATX
	- ITX
	- mITX
- Motherboard connectors types
	- PCI
	- PCIe — type of expansion slot
	- Riser card
	- Socket types
	- SATA
	- IDE
	- Front panel connector
	- Internal USB connector
	- M.2 SSD — SSD connecting via M.2 I guess
- BIOS/UEFI settings
	- **Boot options** — related: correct boot sequence for PC is 
	- Firmware updates
	- Security settings
	- Interface configurations
	- Security
		- Passwords — CMOS password reset by removing shunt from clear CMOS jumper ? 
		- Drive encryption
			- TPM
			- LoJack
			- Secure boot
- CMOS battery
- CPU features
	- Single-core
	- Multicore
	- Virtualization
	- Hyperthreading
	- Speeds
	- Overclocking
	- Integrated GPU
- Compatibility — these squares which we call CPUs just pop out, compatible with specific motherboards
	- AMD
	- Intel
- Cooling mechanism
	- Fans
	- Heat sink
	- Liquid
	- Thermal paste
- Expansion cards
	- Video cards
		- Onboard
		- Add-on card
	- Sound cards
	- Network interface card
	- USB expansion card
	- eSATA card

### 3.6 Explain the purposes and uses of various peripheral types.
- Printer
- ADF/flatbed scanner
- Barcode scanner/QR scanner 
- Monitors
- VR headset
- Optical drive types 
- Mouse
- Keyboard 
- Touchpad 
- Signature pad 
- Game controllers
- Camera/webcam
- Microphone 
- Speakers
- Headset
- Projector
	- Lumens/brightness 
- External storage drives 
- KVM — keyboard video and mouse, many computers connected to one set of KVM
- Magnetic reader/chip reader 
- NFC/tap pay device 
- Smart card reader
- System unit — the big box housing the motherboard, CPU, RAM, hard drives, all else are peripherals #todo find out the name of those hole slots for GPU ports and etc. 

### 3.7 Summarize power supply types and features.
- Input 115V vs. 220V 
- Output 5V vs. 12V 
- 24-pin motherboard adapter 
- Wattage rating 
- Number of devices/types of devices to be powered

### 3.8 Given a scenario, select and configure appropriate components for a custom PC configuration to meet customer specifications or needs.
[configurations.md](configurations.md)

### 3.9 Given a scenario, install and configure common devices.
- Desktop
	- Thin client
	- Thick client
	- Account setup/settings
- Laptop/common mobile devices
	- Touchpad configuration
	- Touchscreen configuration
	- Application installations/configurations
	- Synchronization settings
	- Account setup/settings
	- Wireless settings

### 3.10 Given a scenario, configure SOHO multifunction devices/printers and settings.
- Use appropriate drivers for a given operating system 
	- Configuration settings 
		- Duplex — just means two sided
		- Collate — 1,2,3,1,2,3 instead of 1,1,2,2,3,3 
		- Orientation 
		- Quality 
- Device sharing 
	- Wired 
		- USB 
		- Serial 
		- Ethernet 
	- Wireless 
		- Bluetooth 
		- 802.11(a, b, g, n, ac) 
		- Infrastructure vs. ad hoc — ad hoc means no WAP between computer and printer, it's direct
	- Integrated print server (hardware) 
	- Cloud printing/remote printing 
- Public/shared devices 
	- Sharing local/networked device via operating system settings 
		- TCP/Bonjour/AirPrint 
	- Data privacy 
		- User authentication on the device 
		- Hard drive caching

### 3.11 Given a scenario, install and maintain various print technologies.
- Laser 
	- Imaging drum, fuser assembly, transfer belt, transfer roller, pickup rollers, separate pads, duplexing assembly — imaging drum is what laser hits so that toner attracts to it
	- [printers.md](printers.md)
	- Maintenance: Replace toner, apply maintenance kit, calibrate, clean 
- Inkjet 
	- Ink cartridge, print head, roller, feeder, duplexing assembly, carriage, and belt 
	- Calibrate 
	- Maintenance: Clean heads, replace cartridges, calibrate, clear jams 
- Thermal 
	- Feed assembly, heating element 
	- Special thermal paper 
	- Maintenance: Replace paper, clean heating element, remove debris 
- Impact — dot matrix printers (type of impact printer) commonly use a *matrix* of 24 pins, sometimes 9
	- Print head, ribbon, tractor feed — these printers use a ribbon basically soaked in ink that the pins push onto the paper
	- Impact paper — tractor feeder uses holes along the sides of the paper to align the paper with the printer
	- Maintenance: Replace ribbon, replace print head, replace paper
- Virtual 
	- Print to file 
	- Print to PDF 
	- Print to XPS 
	- Print to image 
- 3D printers 
	- Plastic filament

## 4.0 Virtualization and Cloud Computing
### 4.1 Compare and contrast cloud computing concepts.
- Common cloud models 
	- IaaS 
	- SaaS 
	- PaaS
	- Public vs. private vs. hybrid vs. community 
- Shared resources 
	- Internal vs. external 
- Rapid elasticity 
- On-demand 
- Resource pooling 
- Measured service 
- Metered 
- Off-site email applications 
- Cloud file storage services 
	- Synchronization apps 
- Virtual application streaming/cloud-based applications 
	- Applications for cell phones/tablets 
	- Applications for laptops/desktops 
- Virtual desktop 
	- Virtual NIC

### 4.2 Given a scenario, set up and configure client-side virtualization.
- Purpose of virtual machines 
- Resource requirements 
- Emulator requirements
- Security requirements 
- Network requirements 
- Hypervisor

## 5.0 Hardware and Network Troubleshooting
### 5.1 Given a scenario, use the best practice methodology to resolve problems. 
- Always consider corporate policies, procedures, and impacts before implementing changes

[change.md](change.md)

### 5.2 Given a scenario, troubleshoot problems related to motherboards, RAM, CPUs, and power.
- Common symptoms
	- Unexpected shutdowns
	- System lockups 
	- POST code beeps
	- Blank screen on bootup
	- BIOS time and setting resets 
	- Attempts to boot to incorrect device 
	- Continuous reboots 
	- No power 
	- Overheating 
	- Loud noise 
	- Intermittent device failure 
	- Fans spin - no power to other devices 
	- Indicator lights 
	- Smoke 
	- Burning smell 
	- Proprietary crash screens (BSOD/pin wheel) 
	- Distended capacitors 
	- Log entries and error messages

### 5.3 Given a scenario, troubleshoot hard drives and RAID arrays.
- Common symptoms 
	- Read/write failure 
	- Slow performance 
	- Loud clicking noise
	- Failure to boot 
	- Drive not recognized 
	- OS not found 
	- RAID not found 
	- RAID stops working 
	- Proprietary crash screens (BSOD/pin wheel) 
	- S.M.A.R.T. errors

### 5.4 Given a scenario, troubleshoot video, projector, and display issues.
- Common symptoms 
	- VGA mode 
	- No image on screen 
	- Overheat shutdown 
	- Dead pixels 
	- Artifacts 
	- Incorrect color patterns 
	- Dim image 
	- Flickering image 
	- Distorted image 
	- Distorted geometry 
	- Burn-in 
	- Oversized images and icons

### 5.5 Given a scenario, troubleshoot common mobile device issues while adhering to the appropriate procedures.
- Common symptoms 
	- No display 
	- Dim display 
	- Flickering display 
	- Sticking keys 
	- Intermittent wireless 
	- Battery not charging 
	- Ghost cursor/pointer drift 
	- No power 
	- Num lock indicator lights 
	- No wireless connectivity 
	- No Bluetooth connectivity 
	- Cannot display to external monitor 
	- Touchscreen non-responsive 
	- Apps not loading 
	- Slow performance 
	- Unable to decrypt email 
	- Extremely short battery life 
	- Overheating 
	- Frozen system 
	- No sound from speakers 
	- GPS not functioning 
	- Swollen battery 
- Disassembling processes for proper reassembly 
	- Document and label cable and screw locations 
	- Organize parts 
	- Refer to manufacturer resources 
	- Use appropriate hand tools

### 5.6 Given a scenario, troubleshoot printers.
- Common symptoms 
	- Streaks 
	- Faded prints 
	- Ghost images 
	- Toner not fused to the paper 
	- Creased paper 
	- Paper not feeding
	- Paper jam 
	- No connectivity 
	- Garbled characters on paper 
	- Vertical lines on page 
	- Backed-up print queue
	- Low memory errors 
	- Access denied 
	- Printer will not print 
	- Color prints in wrong print color
	- Unable to install printer
	- Printing blank pages 
	- No image on printer display 
	- Multiple failed jobs in logs

### 5.7 Given a scenario, troubleshoot common wired and wireless network problems.
- Common symptoms 
	- Limited connectivity 
	- Unavailable resources 
		- Internet 
		- Local resources 
			- Shares 
			- Printers 
			- Email 
	- No connectivity 
	- APIPA/link local address 
	- Intermittent connectivity 
	- IP conflict 
	- Slow transfer speeds 
	- Low RF signal 
	- SSID not found

## A+ Proposed Hardware and Software List

### EQUIPMENT
- Apple tablet/smartphone 
- Android tablet/smartphone 
- Windows tablet/Smartphone 
- Chromebook 
- Windows laptop/Mac laptop/Linux laptop 
- Windows desktop/Mac desktop/Linux desktop 
- Windows Server w/Active Directory and Print Management 
- Monitors 
- Projectors 
- SOHO router/switch 
- Access point 
- VoIP phone 
- Printer 
	- Laser/inkjet 
	- Wireless 
	- 3D printer 
- Surge suppressor 
- UPS 
- VR headset 
- Smart devices (IoT devices)

### SPARE PARTS/HARDWARE
- Motherboards 
- RAM
- Hard drives 
- Power supplies 
- Video cards 
- Sounds cards 
- Network cards 
- Wireless NICs 
- Fans/cooling devices/heat sink 
- CPUs 
- Assorted connectors/cables 
	- USB 
	- HDMI 
	- Etc. 
- Adapters 
- Network cables 
- Unterminated network cables/connectors 
- AC adapters 
- Optical drives 
- Screws/stand-offs 
- Cases 
- Maintenance kit 
- Mice/keyboards 
- KVM 
- Console cable

### TOOLS
- Screw drivers — Phillips #2 gets into almost any system
- Multimeter — aka voltage tester or volt/ohm meter or voltmeter???
- Wire cutters 
- Punchdown tool 
- Crimper 
- Power supply tester 
- Cable stripper 
- Standard technician toolkit — nut drivers attach to screw driver to open even more systems, spudgers and pry bars open mobile phones, hemostat picks up dropped screws
- ESD strap 
- Thermal paste 
- Cable tester 
- Cable toner 
- WiFi analyzer
- SATA to USB connectors

### SOFTWARE
- Operating systems 
	- Linux 
	- Chrome OS 
	- Microsoft Windows 
	- Mac OS 
	- Android 
	- iOS 
- PE Disk/Live CD 
- Antivirus software 
- Virtualization software 
- Anti-malware 
- Driver software