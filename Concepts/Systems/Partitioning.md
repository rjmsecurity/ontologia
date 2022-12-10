# Partitioning

- *partitioning* means separating one physical storage drive into logical parts or *volumes* as Windows calls it
	- it's the first step in preparing disks
	- useful for multiple operating systems
	- existing partitions and their file systems may not be compatible with your new OS
	- be careful, there is data loss risk
- *MBR* (master boot record) partition style is the older one
	- *Primary* partitions are bootable by the OS
		- maximum of 4 primary partitions per disk
		- one of which is active
	- *Extended* refers to one extended partition with additional *Logical* partitions, none of which are bootable
- *GPT* (GUID Partition Table) is the newer one
	- GUID means globally unique identifier
	- requires UEFI BIOS (or BIOS-compatibility mode but that disables UEFI SecureBoot and then you can't boot Windows)
	- up to 128 partitions
	- all bootable
- *Dynamic disk* means that partitions can extend across multiple disks
	- modern Windows
	- striping or mirroring
	- make sure you know what options are available for your version of Windows
	- Windows wants to know whether your disk is dynamic or basic before you set the file system type
- *Basic disk* means we're using the primary and extended partitions and logical drives we discussed
	- DOS and Windows
	- can't span partition across drives
- *recovery partition* 
	- takes all Windows installation files and make copy of them to hidden partition
	- used in a repair installation
	- modern Windows does this itself when you install an OS
	- if the recovery partition was not created automatically during the Windows install, you can create one yourself 
	- copy all the files you just used for install into that recovery partition so you don't have to hunt for the install media later
- a *swap partition* is used when many apps are running and there's no more memory left
	- the OS copies unused data to the swap partition in the disk
	- swap partitions are found in the below file systems
	- usually the partition will be on the fastest drive or SSD
- when you install Windows, it'll create four partitions: a Primary, a Recovery, a "System", and an "MSR (Reserved)"

#aplus #core2 **1.3** *Summarize general OS installation considerations and upgrade methods.* 
