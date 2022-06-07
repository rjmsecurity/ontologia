> 1.3 Summarize general OS installation considerations and upgrade methods. 

# Types of installations 

- *unattended installation*
	- all those prompts are pre-answered
	- installation simply goes through entire process without any user intervention
	- answers are provided by you in a file called *unattend.xml*
	- this is useful when you work in corporation with many computers
- *in-place upgrade*
	- some Windows versions (see below table) allow installing newer version on top of older version
	- keep all your apps and config settings in place
	- you're just changing the OS version
- *clean install*
	- opposite of an in-place upgrade
	- you have to move all your apps and settings
	- there are migration tools that help you back up and restore when install is completed
- a *repair installation* reinstalls the same OS to fix a problem with it and leaves all files and apps in place
- *refresh/restore*
	- requires a recovery partition (see below partitions section)
	- Windows 8/10 feature to clean things up
	- how is this different from a repair install?
- *multiboot* means running two or more operating systems from a single computer, choosing which to boot to during boot 
- *remote network installation* I assume refers to PXE or Netboot
- *image deployment* is when you have many computers to deploy a clone to via an image, again I assume this refers to optical discs or USB 

Which Windows versions can upgrade to Windows 10 and which must go through a clean install
From | Windows 10 Home | Windows 10 Pro | Windows 10 Enterprise 
-- | - | - | -
Windows 7 Starter | Upgrade | Upgrade | Install
Windows 7 Home Basic | Upgrade | Upgrade | Install
Windows 7 Home Premium | Upgrade | Upgrade | Install
Windows 7 Professional | Install | Upgrade | Upgrade
Windows 7 Ultimate | Install | Upgrade | Install
Windows 7 Enterprise | Install | Install | Upgrade
Windows 8 (any) | Install | Install | Install
Windows 8.1 Core | Upgrade | Upgrade | Install
Windows 8.1 Professional | Install | Upgrade | Upgrade
Windows 8.1 Enterprise | Install | Install | Upgrade
