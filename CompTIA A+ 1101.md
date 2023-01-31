# CompTIA A+ Core 1 (220-1101)

These objectives are copied from [CompTIA's objectives PDF](https://partners.comptia.org/docs/default-source/resources/comptia-a-220-1101-exam-objectives-(3-0)). Read more [about the A+](CompTIA%20A+%20hardware%20and%20software.md) or see what [resources I used](Resources.md).

## 1.0 Mobile Devices

### 1.1 Given a scenario, install and configure laptop hardware and components.

* Hardware/device replacement
	* Battery
	* **Keyboard/keys ⟹** connect with a ribbon cable ([see image](./images/ribbon_cable.png))
	* Random-access memory (RAM)
	* Hard disk drive (HDD)/solid-state drive (SSD) migration
	* HDD/SSD replacement
		* SSD vs. hybrid vs. magnetic disk
		- **1.8in vs. 2.5in ⟹** 1.8" is M.2 and 2.5" can be either SSD or magnetic, both commonly on laptops
	* **Wireless cards/Bluetooth module ⟹** newer laptops have them in the motherboard, older laptops may have Mini PCI or Mini PCI Express interfaces for you to add wireless connectivity
		* like with replacing hard drives, there may be a cover on the back of the laptop to easily open for you to access these interfaces ([see image](./images/Mini_PCI_Express_interfaces.png))
		* Mini PCI/PCI Express are easy, just slide the wireless card into the slot, usually there's also an antenna wire to connect to the appropriate port on the card ([Messer image at 14:30](https://youtu.be/y7oHZ1mi7e4?t=870)) 

* Physical privacy and security components
	* **Biometrics ⟹** Windows settings > Accounts > Sign-in options
	* [Near-field scanner feature](./Concepts/Networks/NFC.md)

- CompTIA 1001 (old) hardware/device replacement:
	- Smart card reader
	- Optical drive
	- Cellular card
	- Video card
	- Mini PCIe
	- Screen
	- DC jack
	- Touchpad
	- Plastics/frames
	- Speaker
	- System board
	- CPU

### 1.2 Compare and contrast the display components of mobile devices.

- Types  
	- **Liquid crystal display (LCD) ⟹** liquid crystals associated with color filters (RGB) in a grid through which a backlight shines from behind to produce images
		- more about the backlight: 
			- older laptops use fluorescent (CCFL, cold cathode fluorescent lamp) 
				- requires more power and is thicker than LED backlight
				- also, CCFL requires an inverter, a CCFL inverter ([see image](./images/inverter.png))
				- CCFL requires AC but laptop uses DC
				- inverter takes low DC voltage from laptop and converts it to high AC voltage for backlight
			- newer laptops use LED
				- thinner, taking up less space
				- around edge of display OR in matrix ([see image](./images/LED_matrix.png)), you can see this matrix if you pull the front off of the display 
				- display is smart enough to recognize what parts of the display should be lighter or darker and will adjust the lighting depending on the image on the screen
				- so common that many say LED display when referring to an LED-backlit LCD
			- to verify backlight failure, shine flash light on screen and if you can make out information, it's possibly the backlight that needs to be replaced and not the display
				- if CCFL backlight, may just need to replace inverters to restore backlight
				- on some systems you need to replace entire display
				- check documentation for your laptop
		- advantages: lightweight, low power consumption, relatively inexpensive
		- disadvantages: because of the backlight, getting true black is difficult; if backlight fails, it is part of the display itself, making it difficult to repair or replace
		- **In-plane switching (IPS) ⟹** excellent color representation (graphics designers and publishers!), but more expensive than a TN LCD
		- **Twisted nematic (TN) ⟹** very good response times (gaming!), but bad viewing angles—off to the side of the display, the color inverts—you need to look directly at the display
		- **Vertical alignment (VA) ⟹** good compromise between TN and IPS, good color representation but response times are a bit slower than TN
	- **Organic light-emitting diode (OLED) ⟹** newer devices use it so it's less common and a tad more expensive, no backlight, organic compound emits light when provided a current, no backlight needed and no glass on the front needed for protection so display is thinner and lighter, it's flexible, and again to repeat the organic material creates its own light when provided power how cool is that; tablets, phones, and smart devices because of how light and portable OLED is and how good the color representation is... oh yeah, true black
	- also look up MicroLED which promises true black like OLED but has higher brightness and contract and does not have the luminance decay issues of OLED
- Mobile display components  
- **WiFi antenna connector/placement ⟹** display is the tallest component of an open laptop, so it's a perfect place to run wireless antennas; make sure when replacing a display to reconnect not only video components but also antenna wires ([see image](./images/antenna_wires_highlighted.png), primary connection for video on left, on right are wires for 802.11); make sure to follow the same path the previous antennas took to connect all those antennas to the appropriate components on the system board; Wi-Fi main and aux cables: usually main is colored (e.g. blue) and auxiliary (backup) is white
- **Camera/webcam and microphone ⟹** many laptops have them integrated; usually the holes next to the webcam are the microphone  
- **Touch screen/digitizer ⟹** can be resistive or capacitative; inside display is a digitizer that converts analog input onto display from fingers (touch screen) or stylus into digital input

### 1.3 Given a scenario, set up and configure accessories and ports of mobile devices.

- Connection methods  
	- **Universal Serial Bus (USB) ⟹** primary wired connection type, high-speed
		- Type A is the most familiar and often seen on computers, mobile device itself may connect with micro/miniUSB
		- **miniUSB ⟹** older devices, aka Mini-B plug
		- **microUSB ⟹** newer devices, aka Micro-B plug
		- **USB-C** ⟹ even newer than microUSB used on both hosts and devices
			- 24-pins, double-sided
			- the USB standard defines what the plug looks like but you can put many types of signals over that single interface: "Acts as a USB 2.0/3.0/3.1/4.0 connection... Can transmit other signals: DisplayPort signals, HDMI video and audio, Thunderbolt data over a USB-C physical connection" (Messer)
		- also they don't mention Type-B plugs, not to be confused with Mini-B or Micro-B, which you saw used on your cheap DVD player ([see Wikipedia](https://en.wikipedia.org/wiki/USB_hardware))
	- **Lightning ⟹** 8-pin proprietary connection from Apple seen on iPhones and iPads
		- advantages over Micro-USB: higher power output for faster charging, double-sided
	- **Serial interfaces ⟹** DB-9 was the common serial communication interface before the advent of USB
		- also called DE-9, this is a 9-pin connection ([see Wikipedia](https://en.wikipedia.org/wiki/D-subminiature))
		- these serial cables commonly transported RS-232 signals
		- Recommended Standard 232, an industry standard of communication since 1969
		- used for connecting consoles on switches, routers, firewalls, etc.; the serial connection for almost everything on computers back in the day: modems, mice
		- used as a configuration port 
		- use a USB to DB-9 converter cable if you need to configure such a device and your computer has only USB (read: if your computer was made in the 21st century)
	- **[Near-field communication (NFC)](./Concepts/Networks/NFC.md)** 
	- **Bluetooth ⟹** high-speed communication over short distances #converge-later 
		- aka PAN, Personal Area Network
		- wireless earbuds, headphones, car stereo, smartphones and tethering, health monitors, smartwatches, speakers
	- **[Hotspot](./Concepts/Networks/Hotspots.md)** 
- Accessories  
	- **Touch pens ⟹** aka touchscreen pen, touchscreen stylus, capacitive stylus; for note-taking, signatures, or precise selection
	- **Active stylus ⟹** aka digital stylus; for artists; more precision and functionality; programmable buttons; pressure sensitivity / stylus can even hover above screen to register; usually is compatible only with a specific tablet, e.g. Apple Pencil with iPad
	- **Headsets ⟹** can connect wirelessly via Bluetooth or wired via USB, Lightning if you're Apple, or 3.5 mm TRRS (tip-ring-ring-sleeve) connector which is an analog audio jack sending your voice from a microphone or information you need to hear in your headphones through the copper connection
		- TRRS is able to separate the simultaneous audio input and output so that you can speak and listen at the same time
	- **Speakers ⟹** I just realized that speakers, headsets, external trackpads, phones, etc. are all battery powered, they're just rechargeable Li-ion batteries; but yeah speakers, stereo sound, woot
	- **Webcam ⟹** commonly external on desktops, internal on laptops/tablets/phones  
- **Docking station ⟹** minimizes plugging/unplugging of cables when arriving at work or at the home office
	- printers, keyboards, mice, displays plug into the docking station
	- some docking stations support additional adapter cards, if you want to extend hardware functionality of your laptop
- **Port replicator ⟹** like a docking station, but instead of sitting your laptop on it, you use a USB cable to connect to it; usually small and don't support additional adapter cards; also I imagine this can be used not only to speed up connecting ports but also if you have a Macbook like me with only USB-C and need all the other ports: Type-A, HDMI, Ethernet...
- **Trackpad ⟹** replaces mouse on laptops; can be external, e.g. Apple's Magic Trackpad
	- if user has problem with inadvertant mouse clicks and movements, some keyboards have a built-in function key (at the top row) to disable/enable the trackpad on the laptop
- **Drawing pad ⟹** (continuing from touch pens and active styluses) if you have a computer that doesn't have a capacitive display or active touch screen, you can add a touch screen capability with an external drawing pad, e.g. Wacom tablet; combines active stylus with external digitizer; again, for precise input; third-party so it's compatible with many computers and operating systems

<!-- ### 1.3 Given a scenario, use appropriate laptop features.
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
- Port replicator 
- Physical laptop lock and cable lock 
- Rotating/removable screens -->

### 1.4 Given a scenario, configure basic mobile-device network connectivity and application support.

* **Wireless/cellular data network (enable/disable) ⟹** cell phones are called cell phones because they use cellular networks
	* cellular networks are called cellular because geographies are separated into sections, or cells ([Messer image at 0:30](https://youtu.be/9dvxRTL_XOI?t=27))
	* antennas are put at edges of those cells so that we can maintain connectivity wherever we travel; antenna coverage of a cell with certain frequencies
	- **2G ⟹** some of the original cellular networks were called 2G networks; they consisted of two global standards for mobile networking: GSM and CDMA 
	- **Global System for Mobile Communications (GSM) vs. code-division multiple access (CDMA) ⟹** good standards for voice communication but very limited support for sending data over the wireless networks
		- originally circuit-switched networks and had to be upgraded to allow some type of data connectivity, for packet-switching
		- GSM was 90% of the worldwide market early on
			- originally an EU standard
			- coverage wherever you travel in the world
			- in the US, AT&T and T-Mobile were the big GSM players
			- the GSM network allowed you to have all of your phone configurations on a **Subscriber Identity Module**, or SIM card, which you can move from phone to phone and your phone number would follow you depending on where the SIM card happens to be
			- original GSM standard used **multiplexing** to be able to have many people communicating at the same time over the same frequencies; every user got a little "slice" of their own "time"; sending voice communication, data communication, all multiplied by many people in one geographic area
		- CDMA also allowed for multiple simultaneous calls
			- information was sent with unique "codes"; each call used a unique code so that your handset could filter out codes irrelevant to your conversation
			- in the US, CDMA was used by Verizon and Sprint; they controlled what handsets you were able to use on those networks
			- CDMA wasn't popular in other parts of the world or with other providers
	- **3G ⟹** 3rd generation, a newer standard introduced in 1998, allowing for more capabilities with sending data and up to several megabits per second of speed
		- with bandwidth improvement came new capabilities: GPS, mobile television, audio and video streaming, and video on demand
	- **Long Term Evolution (LTE) ⟹** a "4G" technology, a converged standard, so providers that used to be GSM or CDMA could now use one standard LTE to be able to send data over a wireless network
		- why? because it was apparent that the separation between GSM and CDMA posed challenges for users who wanted to move between providers or use different networks available in their area
		- LTE is based on GSM and EDGE (Enhanced Data Rates for GSM Evolution)
		- throughput increased: download up to 150 Mbps
		- some areas have LTE Advanced (LTE-A) which supports up to 300 Mbps
	- **5G ⟹** fifth generation cellular networking, introduced 2020; faster, higher frequencies
		- eventually it will support 10 Gbps, today speeds are slower at 100-900 Mbps
		- as with 3G ushering in GPS and video streaming, 5G will enable new capabilities with IoT, since bandwidth is practically no longer an issue: many devices on home networks, larger file transfers, faster monitoring and notification, uploading more data to cloud for processing (I'm sure Tesla likes the 5G upgrade)
	- **[Hotspot](./Concepts/Networks/Hotspots.md)**  
	- **Preferred Roaming List (PRL) updates ⟹** PRL allows your phone to understand where all of the appropriate towers are for the network you're using
		- allows your phone to connect to the right tower
		- can be updated over the air, or OTA
		- if your phone is performing an OTA update, it may be that a PRL needs to be updated
		- Messer writes but didn't talk about it: *CDMA networks (Verizon, Sprint)*
- Bluetooth #converge-later
	- below are the steps in the Bluetooth pairing process
	1. **Enable Bluetooth ⟹** phone settings 
	2. **Enable pairing ⟹** this process is a security function allowing you to approve devices to connect to phone via Bluetooth
		- only needs to be done once; future connections should be automatic
		- enter **discoverable mode** on the Bluetooth device, usually by holding or pressing a button a number of times; check with manufacturer
	3. **Find a device for pairing**
	4. **Enter the appropriate PIN code** 
	5. **Test connectivity**  
- **Location services ⟹** geotracking; Maps
	- **Global Positioning System (GPS) services** 
		- currently over 30 GPS satellites in orbit, created by the DoD
		- phone needs to see at least 4 satellites in order to give precise location
		- determines longitude, latitude, and altitude based on timing differences between each satellite
	- **Cellular location services ⟹** phones can also use Wi-Fi and cellular towers for more precise location (**triangulation**? like how police trace a call to a location)
- [**Mobile device management](https://youtu.be/zn2Xf9hAFcE?t=466) (MDM)/mobile application management (MAM) ⟹** for management of both company-owned and user-owned (Bring Your Own Device, **BYOD**) devices
	- allows manager of MDM to sit at a single console and gain access to the configurations of all of the mobile devices in their environment
	- especially important to manage security if company data is on the devices
	- policies can ensure apps are installed, data is protected, camera is disabled...
	- ability to **partition** out the company data and protect it differently from personal data
		- this allows for easy deletion of company data without affecting personal data
	- ability to manage access control: force screen lock after timeout, force passcodes
	- **Corporate email configuration ⟹** an MDM makes things like configuring email hassle-free for the user; corporate email configurations can be pushed out from MDM
		- account details, server address, communication method
	- **Two-factor authentication ⟹** require both credentials and biometrics, or company's  pseudo-random authentication app, or other when logging into a service
	- **Corporate applications ⟹** ensure required apps are installed automatically or forbid certain apps 
- Mobile device synchronization  
	- Account setup  
		- **Microsoft 365 ⟹** or Outlook or Exchange if your company is running its own Exchange servers; same for Hotmail 
			- requires authentication to Microsoft 365 with username and password
			- you can synchronize contacts, calendars, reminders, and notes to Microsoft 365 in addition to email
				- so you can start a note on your phone and open on desktop
		- **Google Workspace (formerly G Suite) ⟹** same process as with Microsoft 365
		- **iCloud ⟹** integrated into iOS and iPadOS; authenticate with iCloud username and password and if I'm not mistaken, Apple's own 2FA functionality where your phone gives you a code for the device you're trying to sign in
			- extensive customization of synchronization in Settings > Apple ID > iCloud
			- e.g. mail, pictures, music, video, calendar, contacts
			- this can use a lot of data so you can also control how that data is sent and over what networks (**data caps**)
				- allow cellular or restrict only to 802.11
				- enable/disable network connections (meaning...?)
				- control cellular downloads: automatic; ask if app download is over 200 MB...
				- this is under Settings > App Store
	- Data to synchronize (see above bullets)
		- Mail  
		- Photos  
		- Calendar  
		- Contacts  
		- Recognizing data caps

<!-- ### 1.4 Compare and contrast characteristics of various types of other mobile devices.
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
		- Micro-USB/Mini-USB/USB-C 
		- Lightning 
		- Tethering 
		- Proprietary vendor-specific ports (communication/power) 
	- Wireless 
		- NFC
		- Bluetooth 
		- IR 
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
	- S/MIME 
- Integrated commercial provider email configuration 
	- iCloud 
	- Google/Inbox 
	- Exchange Online 
	- Yahoo 
- PRI updates/PRL updates/baseband updates → prl is preferred roaming list and you should download it if you can't connect to carrier network outside of home, and pri is something something interface I think and it's just updates for something
- Radio firmware 
- IMEI vs. IMSI → imsi identifies phone and network, imei identifies globally unique phone
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
- Connection types to enable synchronization --> 

## 2.0 Networking

### 2.1 Compare and contrast Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) ports, protocols, and their purposes.  

* encapsulation
	* packets traveling across Ethernet networks contain an **Ethernet Payload** with an **Ethernet Header** attached before it and an **Ethernet Trailer** attached after it
	* the Ethernet Payload can contain anything; the most popular thing used on networks is the **Internet Protocol**, which has an **IP Header** and **IP Payload**
	* the IP Payload can contain TCP or UDP; if it's TCP for example then there's a **TCP Header** and **TCP Payload**
	* the TCP Payload can be separated out into different types of data such as **HTTP data**; so for the entire Ethernet frame, inside is IP, inside IP is TCP, and inside TCP is HTTP data ([see Messer image at 2:40](https://youtu.be/YIaF4cJRB4g?t=160))
* IPv4 sockets (Messer didn't explain this word) – for any communication, we need the following information: 
	* server IP address, protocol, server application port number
		* servers/services use **non-ephemeral** ports, or permanent port numbers
			* ports 0-1023
			* e.g. web servers are always ports 80 and 443
	* client IP address, protocol, client port number
		* clients use **ephemeral** ports, or temporary port numbers
			* ports 1024-65535
			* determined in real-time by the client
			* once a traffic flow is over, the OS will no longer use that port number (freeing it up)
	* this isn't strict, port numbers are just that, they're numbers commonly associated with a service
	* they're non-ephemeral and commonly used to make communication faster and simpler
	* again, port numbers are for communication, not for security: using a different, obscure port number for a service doesn't stop a port scanner from scanning for all open ports and further probing each port to find out what service is running 
	* TCP port numbers are different from UDP port numbers but it can create confusion to have both a TCP service and a UDP service running on the same port so people don't do that
	* firewalls usually have rules based on port numbers so that's another reason why it's important to use well-known port numbers; port-based security
* common network ports and protocols (aka **well-known port numbers**) ⟹ [Ports.md](./Concepts/Networks/Ports.md)
* TCP vs. UDP  
	* TCP and UDP are transported inside of an IP packet; they are **encapsulated** within IP
	* operate at the transport layer of the OSI model; at layer 4
	* you may think that IP is all you would need to move data from one part of the network to another; in many ways, you would be correct, but TCP and UDP add additional capabilities that IP can't provide, e.g. **multiplexing**, or the ability to have many different applications on a system simultaneously communicating to a remote server
		* so your workstation is sending a lot of information for a lot of applications to a server and, through multiplexing, the server is able to determine what apps are in use 
	* **Transmission Control Protocol (TCP) ⟹** *connection-oriented* protocol
		* formal process to set up a connection and a formal process to end it when the conversation is over
		* *reliable* delivery — built-in system to verify data was received by recipient
			* recovery from errors
			* can reorder messages received out-of-order which can happen on networks that have multiple links to a single location
			* can manage a retransmission process so that data not received can be resent
		* flow control — if a device feels its receiving information too quickly, it can manage how much data is sent by telling the sender to slow down
	* **User Datagram Protocol (UDP) ⟹** *connectionless* traffic flow
		* no formal process to set up a traffic flow or to tear it down at the end; simply send data from one place to the other
		* *unreliable* delivery — no acknowledgement being sent by the destination device
			* no error recovery
			* no reordering of data or retransmissions
		* no flow control like with TCP — recipient can't slow it down because it's just a one-way conversation from one device to another
		* UDP's weaknesses are its strengths in real-time communication, like in a phone call, where you can't stop and resend a packet, there's no catching up to where you were; time does not stop for your network; you just need to send information very quickly and keep the conversation going if some information is lost along the way
	- Connectionless
		- **Dynamic Host Configuration Protocol (DHCP) ⟹** automatic assigning of IP addresses to devices
			- taking DHCP as an example of an application using UDP: because UDP is unreliable, it is the responsibility of DHCP, the application, to do keep track of responses and do something if it doesn't get a response from the recipient, if it has no acknowledgement; the application can resend the data, or it might decide to do nothing depending on the application
		- **Trivial File Transfer Protocol (TFTP) ⟹** 
	- Connection-oriented
		- continuing off the thought before about UDP applications, taking HTTPS as an example of an application using TLS: if our HTTPS data between a web server and client loses a packet, TCP will recognize it and ask to retransmit that information; HTTPS and SSH don't have to worry about the process of getting data from one side to the other
		- **Hypertext Transfer Protocol Secure (HTTPS) ⟹** 
		- **Secure Shell (SSH) ⟹** encrypted terminal communication between systems
- if IP addresses are the address of a house, port numbers are the rooms of that house where the mail, the packets, need to go
	- port numbers specify which application, aka service, aka server (e.g. web server), that this information is being communicated with
	- again, this is why multiplexing is useful; the IP address receives a lot of packets and the port numbers allow for directing that data to the right services
	- [watch the last two minutes for a good review with pictures](https://youtu.be/YIaF4cJRB4g?t=954)

### 2.2 Compare and contrast common networking hardware.  

![router symbol](https://upload.wikimedia.org/wikipedia/commons/5/55/Router_symbol-Blue.svg)
* **Routers ⟹** forwards traffic between different IP subnets 
	* uses the IP address within a packet to determine the packet's next hop on its way to the final destination
	* because routing takes place on layer 3 of the OSI model, routers are referred to as layer 3 devices
	* if you have a router that can be configured inside of a switch, it's referred to as a **layer 3 switch**
	* SOHO routers are a type of multipurpose networking device, combining the functionality of a switch, router, WAP, firewall... 
		* single-purpose devices are usually found in data centers 
	* routers can connect IP subnets using the same topology and routers can connect different types of networks—the interfaces on a router might connect LAN, WAN, copper, fiber
![network switch symbol](https://upload.wikimedia.org/wikipedia/commons/6/69/Switch_symbol-Blue.svg)
* **Switches ⟹** forwards traffic based on destination *MAC address*, or data link address, inside of a frame
	* forwards at high rates of speed because a lot of the forwarding is done in the hardware itself; many switches have an **Application-specific integrated circuit (ASIC)** which allows for very fast throughput; "bridging is done in the hardware"
	* when you use a copper cable to plug in a laptop or desktop, then you're commonly plugging into a switch
	* if you have a switch that's in the core of an enterprise network, there could be tens or even hundreds of interfaces on that switch
		* many switches will also add additional power to the switch connection using **Power over Ethernet (PoE)** 
	* and again, a switch that can enable additional routing functionality is a layer 3 switch or a **multilayer switch**
	* **Unmanaged ⟹** not a lot of functionality or configuration; simply connecting devices together; plug and play
		* usually purchased from a local or online retailer
		* for your home
		* can't configure VLANs; effectively all connected devices are on one VLAN
		* very little integration with other protocols or devices
			* no management protocols like SNMP
			* network admin can connect unmanaged switch to network but cannot query it to check performance or errors
		* low cost, if all you need is simple connectivity 
		* [Messer image at 3:20](https://youtu.be/1cS5JPULDdY?t=200)
	* **Managed ⟹** support for VLANs, SNMP, STP, port mirroring... many capabilities for network admins who need to constantly monitor and confirm switch is working as expected
		* for offices and enterprises
		* configure different interfaces to be on completely different IP subnets, or **virtual LANS (VLANs)**
			* interconnect with other switches via 802.1Q
		* configuration options to prioritize traffic, e.g., set VoIP traffic to have a higher priority than file transfer traffic
		* common for organizations to connect multiple switches to their network, and **Spanning Tree Protocol (STP)** prevents loops between all of those switches; redundancy support
		* **port mirroring**, or taking traffic from one port on the switch and copy all of that traffic to a different port on the switch, ideally to plug in a **protocol analyzer** to be able to view all the packets traversing the network
			* commonly used for troubleshooting and packet analysis 
		* SNMP for external management
		* [Messer image at 3:50](https://youtu.be/1cS5JPULDdY?t=230)
* **Access points ⟹** provides wireless connectivity for the local network
	* not a router that you might find in a SOHO device, it's a device that only provides a link between the wireless network and the wired network
	* aka a **bridge** because they are simply bridging or extending that wired connection into a wireless connection
	* doesn't route between subnets or perform any NAT
	* forwarding is based on the destination MAC address, similar to a switch
		* determines whether that MAC is on the wireless network or if it should send the information to the wired network
	* can look like a white square stuck to the ceiling ([Messer image at 4:59](https://youtu.be/1cS5JPULDdY?t=299))
	* a **wireless router** is a router and an access point in one device
* **Patch panel ⟹** 
	* connecting many people in a work environment means managing a lot of cables
	* all the cables from each office on a floor of a building **run** to a central wiring closet on that floor
	* in that wiring closet is a patch panel; first connect all those cables from each office to the patch panel...
		* that run is a permanent run; we don't tend to move those cables 
	* ...on the other side of the patch panel can be connectors like RJ-45 connectors
		* [Messer image at 7:30 shows the RJ-45 side of a patch panel](https://youtu.be/1cS5JPULDdY?t=452)
		* extend those RJ-45 connector to interfaces that may be on a switch inside of that wiring closet
		* [Messer image at 8:20 showing the connections between a patch panel and a switch](https://youtu.be/1cS5JPULDdY?t=502)
		* at this point, somebody's office desk is connected back to the main network infrastructure
		* if a person moves desk or a new hire sits at a new desk; in those scenarios you may have to move someone from a connection on one switch to a connection on another switch
		* the patch panel allows you to simply disconnect from one switch and reconnect that RJ-45 port on the patch panel to a different switch (instead of having an entire cable running from the desk to the switch that needs to be moved)
		* shorter, labled cable so you know exactly which desk it's going to, faster changes
			* limits the scope of any problems that might occur during changes
	* again, the wiring between a workstation and the closet doesn't change
		* it's **punched down** and permanently connected to the back of the patch panel
		* in Messer's notes it says it's punched down onto a **110 block**
		* aka **punch-down blocks**
	* [Messer image at 6:05](https://youtu.be/1cS5JPULDdY?t=372)
* **Firewall ⟹** allow or disallow traffic through your network based on IP addresses and port numbers
	* since TCP and UDP ports operate at layer 4 of the OSI model, it's common to refer to firewalls as an OSI **layer 4 device**
	* these days it's increasingly common to have firewalls understand application layer traffic, and in those cases the firewall is a **layer 7 device**
	* some firewalls can also act as an **endpoint for an encrypted tunnel**
		* encrypting traffic into/out of the network
		* you can connect two **sites** together across a public network like the internet and all of the traffic between those sites is encrypted
	* some can also act as a **proxy**; if someone is browsing a site on the internet, the firewall will stop that communication, it will perform the browsing for the user, receive the response from that device over the internet, examine and make sure nothing inside of that traffic may be dangerous or malicious, and then send the results of that query back to the user
	* some can also act as a **router**; common with SOHO routers; making forwarding decisions based on the destination IP address, acting as an OSI layer 3 device
		* in many environments, the firewall is the device connected directly to the internet, so using it also as a router allows additional functionality for forwarding traffic
		* aka firewalls usually sit on the **ingress**/**egress** of the network
* **Power over Ethernet (PoE) ⟹** run a single wire to a device that will not only be able to transfer data but also used as the power source for that device
	* used with access points, cameras, phones, and any thing else where power may be difficult to run to that device
	* useful in difficult-to-power areas; one wire for both network and electricity
	* **endspans** are where the power is coming directly from the switch
		* built-in power
	* **midspan** aka **injector** is for when your switch doesn't support PoE and you need something in the middle of the connection to add power to the Ethernet cable
		* in-line power injector
		* [Messer image at 11:00](https://youtu.be/1cS5JPULDdY?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=665)
		* so for example you have a PoE injector with an RJ-45 jack labeled PoE/DATA for your camera, another jack labeled DATA IN for your switch that doesn't support PoE, and a power source for the injector; that way your camera can receive its power and data (is it sending or receiving data over Ethernet? or both)
	* **PoE switch ⟹** most switches will mark what interfaces can support PoE
		* [Messer image at 11:25](https://youtu.be/1cS5JPULDdY?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=685) showing a common 8-port Ethernet switch; across the top is a blue line and anywhere that blue line is, the port supports PoE
			* in this example it's ports 1-8 and there's a port 9 that looks like it's commonly used as an [**uplink port**](https://www.google.com/search?q=uplink+port) and it doesn't have the blue line painted above it so it doesn't support PoE
	* **PoE standards ⟹** 
		* different devices need different types of power
		* there are different standards for PoE depending on what type of switch you might be using
		* **PoE: *IEEE 802.3af-2003* ⟹** original PoE specification from 2003 
			* has now been rolled in to the standard 802.3 Ethernet standard
			* provides 15.4 watts of DC power with 350 mA (milliamps) as the max current
		* **PoE+: *IEEE 802.3at-2009* ⟹** introduced 2009 
			* also been wrapped in to 802.3 standard
			* provides 25.5 watts of DC power with max current of 600 mA
		* **PoE++: *IEEE 802.3bt-2018* ⟹** introduced 2018
			* it's referred to as Type 3 when we're providing 51 watts with 600 mA of max current
			* Type 4 PoE++ is 71.3 W and 960 mA max current
			* this standard is designed to work with 10GBASE-T (10 gigabit per second Ethernet) and provide power for those 10 gig devices
* **Hub ⟹** aka *multi-port repeater*
	* before switches, hubs connected all devices on networks
	* not very intelligent devices, hence the nickname above
	* any data going into one interface is automatically copied and sent to other interfaces on the hub
	* so as you put more of a load and add more devices to the network, the performance of the hub tends to get slower and slower
	* inefficient communication; as network traffic increases, hub efficiency decreases
	* no ability to run **full-duplex** (?) communication to a hub
	* so all devices plugged in to the hub will operate at **half-duplex**
	* only available in 10 megabit and 100 megabit speeds
	* hubs are outdated devices and only available on a secondary or used markets
* **Cable modem ⟹** communicates over **broadband**
	* uses same cable for your internet connection as your cable television
	* broadband is called that because there are multiple frequencies of traffic being used over a single wire
		* we can have video signals for television
		* we can connect our phone lines into this cable modem
		* and it can be used for internet data
		* so you can have these multiple services with cable modems
	* **DOCSIS** (Data Over Cable Service Interface Specification) is the standard for sending data over these cable networks
	* speeds up to 1 Gigabit/s, yours depends on your service provider
	* there are usually multiple services available on these networks and when you connect the cable, you can either connect to the data that's on the internet side (I think Prof. is referring to the RJ-45 connector on the back of the modem, separate from the coax connection above it)... the [cable modem shown at 15:00](https://youtu.be/1cS5JPULDdY?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=909) also has analog telephone connections for any voice communication (I think he means the RJ-11)
* **Digital subscriber line (DSL) ⟹** uses the traditional telephone company to provide internet 
	* if you're not using your cable company
	* also called a modem, a DSL modem
	* often technically **ADSL (Asymmetric Digital Subscriber Line)**
	* uses the same telephone lines that we've always used for our analog telephone
	* the reason it's asymmetric is because the download speeds are faster than the upload speeds
	* 52 Mbit/s downstream and 16 Mbit up
	* but you can find larger and faster DSL implementations depending on the capabilities from your provider
	* distance limitation with DSL before the signal gets so weak that you can't receive any of the data
	* usually around ~10,000 feet from the central office (CO)
	* if you are closer to the CO, you tend to get faster throughput than when you are farther away
* **Optical network terminal (ONT) ⟹** connection to the fiber network
	* if you are not connecting to the internet using copper cable or telephone lines
	* a device usually connected to the outside of your home/building/premise, terminal box on side of building
	* fiber to the premises
	* connecting an ISP fiber network and converting it into signals like copper Ethernet that can be used inside your home
	* delineates the ISP's network from your own internal network
	* we refer to this delineation as the **demarcation point**, or simply **demarc**
	* sometimes this demarc is located in your data center itself or if you're at home it's located on the outside of your home
	* it's important that a demarc exists so that you know what the responsibilities are for each different party
		* you know that any of the wiring on the inside of your house is your responsibility up to the point of that demarc 
		* anything outside that demarc is the responsibility of the service provider
	* [17:10 shows an image of an ONT](https://youtu.be/1cS5JPULDdY?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=1035) with:
		* the fiber connection coming from the street and the fiber label over it
		* outputs for data (Ethernet connection)
		* analog telephone connections
		* F connector for cable connection for your television (coax)
* **Network interface card (NIC) ⟹** the fundamental network device
	* every device on a network has a NIC
	* computers, servers, printers, routers, switches, phones, tablets, cameras
	* if you are connecting to a copper Ethernet connection, you're using a NIC to provide that connectivity
	* all devices discussed in this section that are connecting to a wired Ethernet connection have a NIC inside of them
	* see image at 18:00 of a NIC you would plug into a server, with four separate Ethernet connectors on the back
	* if you have a laptop or desktop computer with an Ethernet interface, that too is a NIC
	* there are NICs for other types of topologies too: if you're plugging into a WAN serial connection, or you have a wireless interface, those also have interface cards
	* these are sometimes built in to the motherboard or it may be a separate adapter, an expansion card, that you plug in to an expansion slot to increase the capabilities of your device
	* so whether you need copper connectivity, fiber connectivity, or anything in between, you will need a NIC on your device to make that connection to the rest of the network
	* copper, fiber, single port, multi-port, many options
* **Software-defined networking (SDN) ⟹** 
	* cloud computing has changed networking
	* in the cloud, there are no physical routers, switches, and other infrastructure devices
	* instead, we need to take these networking platforms we use in the real world and move them into the virtualized, cloud-based world
	* with SDN, we take those switches, routers, firewalls, and other networking infrastructure devices and we change them to be a software-based platform that we could use in the cloud
	* we can take something like a switch and separate all the functions of the switch into individual pieces
	* we can then take these pieces and create software versions that we can run in the cloud
	* networking devices have different functional planes of operation: data, control, and management planes
	* so we split the functions into separate logical units, extending the functionality and management of a single devices, perfectly built for the cloud
	* three layers or ways to separate these devices to create some consistency across all of these networking components
	* the first layer is the **infrastructure layer** aka the **data plane** of a device
		* data plane does the forwarding, the trunking (?), the encrypting, the NAT, anything that needs to occur at the packet level
		* process the network frames and packets
	* when our routers and switches need to forward this traffic in the data plane, they need some type of reference to know where this traffic will be going
	* most of those references will be in the **control layer** or the **control plane** of that device
		* if you have dynamic routing protocol updates, a forwarding table in a switch, routing tables, session tables, a NAT table in a router, all of those are contained in the control plane
		* manage the actions of the data plane
	* you or some other process is in charge of configuring and managing that device
	* to be able to manage it, we need to log in or access the device via an API 
	* all of that access is provided at the **application layer** or **management plane** of that device
	* so when you SSH into a router or bring up a graphical front end of a firewall in your browser, you're managing that device from the management plane
	* [see 2:10 for an image of a physical device](https://youtu.be/wNiDqwCoojI?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=137) and how SDN applies 
		* could be a switch, a router, a firewall, or any other infrastructure device
		* if you're connecting to a switch or you need traffic forwarded between different interfaces on the switch, that all occurs in the data plane (to me it looks like RJ-45 ports and some other ports 1-32 are highlighted as part of this plane)
		* we will take anything that may be forwarding traffic on the device and create a software version of that called the data plane
		* these devices also need the tables and forwarding structure to be able to understand where traffic is coming from and where you will be forwarding it to, and all of that occurs in the control plane (top part of the device is highlighted, nothing really, but it represents the control plane in the image—the brain of the device?)
		* you will be managing this device probably through a console port or management interface to the device, and that section of the device can be created as the management plane (left part of device highlighted, with said console port and a couple other ports labeled MGMT1 and 2 and USB ports)
		* obviously with SDN there is no physical device, but you can see where the data plane, control plane, and management plane are pulled from our physical devices to create this software-based networking infrastructure
	* this now creates modular layers that you can extend between devices or create new devices, all based on this SDN
	* [see image at 3:30](https://youtu.be/wNiDqwCoojI?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=210) e.g. if we start at the bottom, we know that network traffic will be traversing different devices all at the data plane
		* a device may need to send or receive dynamic routing protocols or create tables for forwarding, and all of those can be done at the control layer of SDN
		* the layer you're going to manage these devices from will be the management plane, we usually access it through SSH, SNMP, or an API
		* so SDN takes these very standard categorizations and extends them across multiple networking devices to create a very modular architecture, allowing you to have a software-based version of these network devices that we use on our physical networks and be able to deploy them and use them in a cloud-based infrastructure

<!-- ### 2.2 Compare and contrast common networking hardware devices. 
- [OSI.md](Concepts/Networks/OSI%20model.md)
- Routers
- Switches 
	- Managed
	- Unmanaged
- Access points
- Cloud-based network controller 
- Firewall
- Network interface card
- Repeater
- Hub
- Cable/DSL modem
- Bridge
- Patch panel
- Power over Ethernet (PoE)
	- Injectors
	- Switch
- Ethernet over Power -->

### 2.3 Compare and contrast protocols for wireless networking.

* the standards for wireless networks come from an IEEE LAN/MAN Standards Comittee called the **IEEE 802** committee and the wireless networking part of this committee is the **802.11** standard
* many updates over time, check with IEEE for the latest
* instead of referring to them as 802.11 wireless networks, you can call it a **Wi-Fi** network
	* this is a trademark from the Wi-Fi Alliance who is responsible for testing the interoperability of all of these different wireless devices
Standard | Frequencies | Maximum MIMO streams | Max theoretical throughput (per stream) | Max theoretical throughput (total)
-- | - | - | - | -
802.11a | 5 GHz | No MIMO support | 54 Mbit/s | 54 Mbit/s
802.11b | 2.4 GHz | No MIMO support | 11 Mbit/s | 11 Mbit/s
802.11g | 2.4 GHz | No MIMO support | 54 Mbit/s | 54 Mbit/s
802.11n | 5 GHz / 2.4 GHz | 4 x MIMO | 150 Mbit/s | 600 Mbit/s
802.11ac | 5 GHz | 8 x DL MU-MIMO | 867 Mbit/s | 6.9 Gbit/s
802.11ax | 5 GHz / 2.4 GHz | 8 x DL and UL MU-MIMO | 1,201 Mbit/s | 9.6 Gbit/s
\*DL means downloadable streams, UL means upload streams (*802.11ac supports 8 downloadable streams of multi-user multi-input multi-output*; *802.11ax supports 8 streams but the multi-user MIMO in ax supports 8 download AND upload streams simultaneously*)
* **802.11a ⟹** one of the very first wireless standards, released Oct 1999
	* operates in the **5 GHz** frequency range
	* can use other frequency ranges with special licensing
	* these days you don't often see many 802.11a networks still around
	* operates at **54 megabits per second**
	* although it doesn't seem fast, back in 1999 when this was first released that was a great deal of speed on a network that suddenly was able to operate wirelessly
	* because we are operating at 5 GHz frequencies, we do not tend to have the same range as lower frequencies such as the 2.4 GHz range that's used by 802.11b
	* with higher frequencies the objects around us tend to absorb the signals, whereas with 802.11b they tend to bounce off of those objects and therefore we get a little bit more distance from a 2.4 GHz-based network
	* it's not common to see 802.11a in use these days and very often this will be a type of network that has already been upgraded to a much faster and newer standard
* **802.11b ⟹** also an original 802.11 standard, released Oct 1999
	* not an upgrade to 802.11a, but a completely different standard that operates with different frequencies and different speeds
	* operates in the **2.4 GHz** range
	* maximum speed is **11 Mbit/s**, much slower than the 54 Mbit/s with 802.11a
	* why choose a slower wireless standard? 2.4 GHz frequencies tend to bounce off of devices instead of being absorbed and therefore we get a bit longer distance in 2.4 GHz networks; **better range**
	* depends on the type of environment: if you are in a warehouse, you may choose 802.11a because there is so much open space
		* if you are in an office setting with a lot of people and desks, you may choose 802.11b because that frequency works a lot better in that environment
	* one challenge we have with this 2.4 GHz range is that wireless networks are not the only devices that can use those frequencies—it's common to see things like baby monitors, cordless phones, microwave ovens, or even the Bluetooth standard take advantage of 2.4 GHz frequencies
	* this means that we could have **frequency conflicts** when trying to communicate using all of these devices simultaneously in one single area
	* it's also difficult to find 802.11b networks that might still be operating, and if you do run into an 802.11b network it's probably because you're upgrading it to a newer version
* **802.11g ⟹** one of the first upgrades available to 802.11b networks
	* June 2003
	* operates in the **2.4 GHz** range
	* increased the speed to **54 Mbit/s**, the same as 802.11a
	* **backwards-compatible with 802.11b**, meaning we can upgrade our access point to the 802.11g and still continue to use our b devices on the same network
	* although 802.11g operates at higher speeds, it still suffers from the same **frequency conflicts** that we had with 802.11b because all of these devices are using 2.4 GHz frequencies
* **802.11n (Wi-Fi 4) ⟹** effectively upgraded 802.11a, b, and g 
	* Oct 2009
	* it's confusing to keep track of all of these different letters and numbers, so instead of using the standard name of 802.11a or 802.11g, we now refer to these standards as "Wi-Fi standards"
		* 802.11n can also be called Wi-Fi 4
		* technically speaking, 802.11a, b, and g can also be called Wi-Fi 1, 2, and 3
		* but because those standards are so old and difficult to find implemented on anyone's networks these days, we are starting with Wi-Fi 4 as the standard for this numbering scheme
	* operates at **5 GHz and/or 2.4 GHz** (simultaneously if your access point supports that)
	* also have more bandwidth available for each individual channel
		* can have up to **40 MHz channel widths**
		* meaning we are able to transfer much more data at the same time over this network
	* if you do have a WAP that is able to use those 40 MHz channel widths and has four antennas on it, you can get a maximum theoretical throughput of **600 Mbit/s**
		* **40 MHz mode and 4 antennas**
	* introduced a new form of communication for wireless networks called **MIMO** (multiple-input multiple-output)
		* devices can transfer much more information simultaneously between the end station and the access point
		* multiple transmit and receive antennas
* **802.11ac (Wi-Fi 5) ⟹** Jan 2014 improvement over 802.11n
	* operates exclusively in the **5 GHz** band, no 2.4 GHz available
		* less crowded, more frequencies—can use much more of that wireless spectrum simultaneously because 802.11ac supports **160 MHz of a channel bandwidth**
		* translates into more channels that can be used simultaneously and therefore more data that can be transferred over the wireless network simultaneously
	* also changes *how* information is transferred over the wireless network, referred to as **signaling modulation**
		* this also increased the amount of data that is able to be transferred at any particular time
	* so it increased **channel bonding** (?), with larger bandwidth usage, and has denser signaling modulation, with faster data transfers
	* not only uses MIMO but increases the capabilities of that MIMO by adding **MU-MIMO** (multi-user MIMO)
		* so multiple users can be communicating over multiple-input multiple-output simultaneously
		* supports up to 8 of those MU-MIMO streams which translates to a maximum total throughput of nearly **7 gigabits per second** 
		* twice as many streams as 802.11n
		* 8 MU-MIMO *downlink* streams (?)
	* if you look at access points that may be available to buy, you will see some of them say that they are 802.11ac access points that operate at 5 GHz and 2.4 GHz
		* in those cases, the communication that's occuring at 2.4 GHz is actually using the 802.11n standard and anything at 5 GHz is using the ac standard
* **802.11ax (Wi-Fi 6) ⟹** Feb 2021 upgrade to 802.11ac
	* operates at either **5 GHz** frequencies or **2.4 GHz** frequencies and on some access points can use both of those simultaneously
	* also supports many different channel widths
		* can have **bandwidths of 20, 40, 80, and 160 MHz** for people communicating on the wireless network
	* total throughput per channel of 1,201 Mbit/s (1.2 Gbit/s)
	* 8 bi-directional MU-MIMO streams
	* relatively small increase in throughput when compared to previous improvements to the standards
	* but 802.11ax was designed to solve some of the problems with using these wireless networks in areas where there are a large number of people
		* if you were at a sporting event or a trade show (or watching Steve Jobs reveal a new iPhone), you may have found it difficult to communicate over these wireless networks
		* 802.11ax introduces a new form of communicating called **orthogonal frequency-division multiple access (OFDMA)**
		* this takes a type of communication that we have used for some time on our cellular networks and brings it into the world of 802.11
		* allows us to put 802.11ax networks in places with large numbers of people and be able to communicate without a huge loss in efficiency over those wireless networks
		* "improves high-density installations"  
* Long-range fixed wireless  
	* if you purchase an access point, bring it home, and plug it in, you will probably get a range of about 40-50 meters if you are using the built-in antennas, the stock antennas
		* if you are working in a corporate environment and you want to connect two buildings together with 802.11, maybe two buildings located miles from each other, then obviously that type of antenna is not going to work
		* instead, you will need some **fixed directional antennas** and you may need to increase the overall signal strength of the 802.11 signal
	* in our offices and homes, we have signals that might be bouncing or be absorbed by the things around us; when we are sending a signal between buildings, there is usually not much in the way that would cause signal absorption or bounce
		* we would use very directional antennas, like the [Yagi antenna at 12:45](https://tryhackme.com/resources/blog/month-in-cyber-january-2023), to be able to have a very focused point-to-point connection between an antenna on one building and the antenna on the other building
	* if you are planning to set up a long-range fixed wireless network, make sure you check the rules and regulations in your area; refer to your country's regulatory agency
		* wireless networks have their own complexities associated with them and when you layer on local and federal rules and regulations regarding wireless communication, it provides some additional complexity to the implementation
		* if you are using a wireless service that is transmitting to your home or you are trying to connect different wireless services between buildings, you may want to look to see what frequencies are available to use 
		* you may have unlicensed 2.4 and 5 GHz frequencies available natively in the standard, but there may be other frequencies available that you can apply for (additional licensing may be required), which might provide you some advantages over using the busier 2.4 GHz or 5 GHz frequencies
		* check with the 802.11 standards and see what options might be available for the type of network that you are installing
	* signal strength: not only are there rules and regulations about what frequencies you can use and where you can use them, there are also regulations about how much of the signal can be sent
		* there are different regulations on whether these signals will be inside of the building or outside of the building, so many sure you know all of the differences when you are installing the network; indoor and outdoor power is usually regulated
	* ultimately, you will need to install an antenna outside if you are receiving a signal from a service provider or you are connecting two buildings together
		* installing antennas outside has its own set of safety requirements, not only in where you install the antenna and that it's not near any power source, but you also have to make sure the antenna is protected in case it happens to be hit by lightning
		* in many cases it might make more sense to bring in a third party who has an expertise in installing these types of external, outdoor networks; outdoor antenna installation is not trivial, get an expert and be safe
	- Licensed  
	- Unlicensed  
	- Power  
	- Regulatory requirements for wireless power  
* **Radio-frequency identification (RFID) ⟹** 
	* access badge that unlocks a door by holding it up to a sensor probably uses RFID inside of the badge
	* extensively used in assembly lines and inventory management in manufacturing 
	* lost pets have RFID chips for scanning and identification
	* i.e. anything that needs to be tracked
	* [15:30 for an image of a cylindrical RFID tag the size of a grain of rice followed by an image of a flat RFID tag that goes inside an access badge](https://youtu.be/-8S9ocPswCE?list=PLG49S3nxzAnnOmvg5UGVenB_qQgsh01uC&t=934)
		* antennas are around the outside and the chip is in the middle
	* no battery; uses radar; antennas capture radio signals which are converted to power added to the chip, allowing the device to transmit back
		* RF powers the tag, ID is transmitted back
		* bidirectional communication
	* there are other RFID tags that do have a power source, those formats are called **active** or **powered** RFID
* [NFC](./Concepts/Networks/NFC.md)  
* Frequencies
	- 2.4GHz  
	- 5GHz  
* Channels  
	- Regulations  
	- 2.4GHz vs. 5GHz  
- Bluetooth  

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
	- UPnP
	- Allow list/deny list
	- MAC filtering
- QoS
- Wireless settings
	- Encryption
	- Channels
	- QoS

==REMINDER: One section at a time, copy over the 1101 objectives to here==

### 2.4 Compare and contrast wireless networking protocols.
- 802.11(a, b, g, n, ac)
- Frequencies
	- 2.4Ghz
	- 5Ghz
- Channels
	- 1-11
- Bluetooth → aka PAN, range about 10m
- NFC → about 10cm range
- RFID
- Zigbee → this and Z-Wave are for internet of things
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
	- Proxy server
	- Mail server
	- Authentication server
	- syslog
- Internet appliance
	- UTM
	- IDS
	- IPS
	- End-point management server
- Legacy/embedded systems

### 2.6 Explain common network configuration concepts. 
- IP addressing
	- Static
	- Dynamic
	- APIPA → address range is ***169.254***.0.1 to ***169.254***.255.254 but since the first and last 256 addresses are reserved it's ***169.254***.1.0 to ***169.254***.254.255
	- Link local
- DNS
- DHCP
	- Reservations
- IPv4 vs. IPv6
- Subnet mask
- Gateway
- VPN
- VLAN
- NAT

### 2.7 Compare and contrast Internet connection types, network types, and their features.
- Internet connection types
	- Cable → uses cable TV lines, up to 300 Mbps
	- DSL
	- Dial-up
	- Fiber → SMF goes longer distances and uses laser so more expensive, MMF uses LED
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
	- WMN

### 2.8 Given a scenario, use appropriate networking tools. 
- Crimper
- Cable stripper
- Multimeter
- Tone generator and probe
- Cable tester
- Loopback plug
- Punchdown tool
- WiFi analyzer

## 3.0 Hardware

### 3.1 Explain basic cable types, features, and their purposes.
- Network cables
	- Ethernet
		- Cat 5
		- Cat 5e
		- Cat 6
		- Plenum → counterpart to PVC which poisons when burned; plenum shielding is safe, more expensive, rated for plenum which refers to the air ducts above office rooms
		- Shielded twisted pair
		- Unshielded twisted pair
		- 568A/B → green and orange are switched
	- Fiber → fyi this isn't just for ethernet but some headphones have fiber connectors
	- Coaxial
	- Speed and transmission limitations
- Video cables
	- VGA
	- HDMI
	- Mini-HDMI
	- DisplayPort → has that notch on one corner
	- DVI (DVI-D/DVI-I)
- Multipurpose cables
	- Lightning
	- Thunderbolt → looks like USB-C ? lightning symbol
	- USB
	- USB-C
	- USB 2.0
	- USB 3.0
- Peripheral cables
	- Serial → 9 pin RS-232 connector
- Hard drive cables
	- **SATA ⟹** seems to be the most common
	- IDE
	- SCSI
- Adapters
	- DVI to HDMI
	- USB to Ethernet
	- DVI to VGA

### 3.2 Identify common connector types.
- RJ-11 → RJ-11 has 6, RJ-45 has 8... I forgot of what, RJ-11 is like a thinner and taller RJ-45
- RJ-45 → network cable connections
- RS-232 → 9 pin, for serial ports
- BNC
- RG-59
- RG-6
- USB → (type A)
- Micro-USB
- Mini-USB
- USB-C
- DB-9 → exactly like RS-232... oh no i can't do this anymore
- Lightning
- SCSI
- eSATA
- Molex → voltages: 
- DisplayPort → has diagonal notch on one corner
- Mini DisplayPort → found on laptops, like a small fat rectangle
- HDMI → you know what it looks like
- mini-DIN (PS/2) → round (and old, but having a renaissance), keyboards and mice
- Parallel port (LPT port) → exclusively for printers 
- Serial port
- VGA → old, monitors

### 3.3 Given a scenario, install RAM types. 
- RAM types
	- SODIMM ⇒ common on laptops
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
- **Solid-state drives** **⟹** solid-state means just that, solid state, no moving parts; silent and faster; can upgrade from hard drive to SSD if same form factor
	- **M.2 drives** **⟹** 1.8" form factor; no SATA cable, so you have drives with a *SATA connection* or with an *M.2 interface*; just plug into a slot like you would a RAM stick and screw a bolt, very modular ([see image](./images/SATA_vs_M.2_interface.png))
	- NVME
	- **SATA 2.5** **⟹** I'm assuming 2.5 refers to inches, 2.5" SSDs use SATA data/power cables ([see image](./images/SATA_vs_M.2_interface.png))
- **Magnetic hard drives (or just *hard drives*) ⟹** older computers; replacing with SSD is a common replacement to improve laptop performance, one way to migrate is to install OS on new drive and manually move all documents, install apps, and personalize settings; a faster way is to clone, or create an image of current hard drive and move image to new SSD; examples of imaging software to achieve this are CloneZilla and Macrium Reflect, SSD manufacturer may also provide their own; organizations like to use image files to create multiple copies; finally there's a drive-to-drive image, the name is misleading because there's no image file, just copying sector by sector directly from one drive to another, by having two systems running simultaneously or one system that can support two drives simultaneously
	- 5,400rpm
	- 7,200rpm
	- 10,000rpm
	- 15,000rpm
	- Sizes:
		- **2.5** **⟹** laptops; when replacing usually it's a couple screws; also the place on the laptop into which you insert an SSD or hard drive is known as a *bay* or drive bay; either it's an access cover on the back of the laptop or you remove the entire back
		- **3.5** **⟹** desktops; also an SSD form factor
- Hybrid drives
- Flash
	- SD card
	- CompactFlash
	- Micro-SD card
	- Mini-SD card
	- xD
- Configurations
	- [RAID.md](Concepts/Systems/RAID%20arrays.md)
	- Hot swappable

### 3.5 Given a scenario, install and configure motherboards, CPUs, and add-on cards.
- Motherboard form factor
	- ATX
	- mATX
	- ITX
	- mITX
- Motherboard connectors types
	- PCI
	- PCIe → type of expansion slot
	- Riser card
	- Socket types
	- SATA
	- IDE
	- Front panel connector
	- Internal USB connector
	- M.2 SSD → SSD connecting via M.2 I guess
- BIOS/UEFI settings
	- Boot options → related: correct boot sequence for PC is 
	- Firmware updates
	- Security settings
	- Interface configurations
	- Security
		- Passwords → CMOS password reset by removing shunt from clear CMOS jumper ? 
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
- Compatibility → these squares which we call CPUs just pop out, compatible with specific motherboards
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
- KVM → keyboard video and mouse, many computers connected to one set of KVM
- Magnetic reader/chip reader 
- NFC/tap pay device 
- Smart card reader
- System unit → the big box housing the motherboard, CPU, RAM, hard drives, all else are peripherals #todo find out the name of those hole slots for GPU ports and etc. 

### 3.7 Summarize power supply types and features.
- Input 115V vs. 220V 
- Output 5V vs. 12V 
- 24-pin motherboard adapter 
- Wattage rating 
- Number of devices/types of devices to be powered

### 3.8 Given a scenario, select and configure appropriate components for a custom PC configuration to meet customer specifications or needs.
[configurations.md](Concepts/Systems/Custom%20configurations.md)

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
		- Duplex → just means two sided
		- Collate → 1,2,3,1,2,3 instead of 1,1,2,2,3,3 
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
		- Infrastructure vs. ad hoc → ad hoc means no WAP between computer and printer, it's direct
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
	- Imaging drum, fuser assembly, transfer belt, transfer roller, pickup rollers, separate pads, duplexing assembly → imaging drum is what laser hits so that toner attracts to it
	- [printers.md](Concepts/Systems/Printing%20process.md)
	- Maintenance: Replace toner, apply maintenance kit, calibrate, clean 
- Inkjet 
	- Ink cartridge, print head, roller, feeder, duplexing assembly, carriage, and belt 
	- Calibrate 
	- Maintenance: Clean heads, replace cartridges, calibrate, clear jams 
- Thermal 
	- Feed assembly, heating element 
	- Special thermal paper 
	- Maintenance: Replace paper, clean heating element, remove debris 
- Impact → dot matrix printers (type of impact printer) commonly use a *matrix* of 24 pins, sometimes 9
	- Print head, ribbon, tractor feed → these printers use a ribbon basically soaked in ink that the pins push onto the paper
	- Impact paper → tractor feeder uses holes along the sides of the paper to align the paper with the printer
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

[change.md](Concepts/Business/Change%20management.md)

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