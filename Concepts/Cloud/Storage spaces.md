# Disk Management: storage spaces

- Windows feature for cloud based systems and data centers
- lets you easily add or remove storage space
- there are tiers of space you can make available with different administrative control
- first a *storage pool* is created, a group of storage devices you have put together
	- you can combine many types of drives with different sizes to create one large pool of storage 
	- and you can add or remove drives to and from that pool as needed
- the next step is creating the actual storage *spaces* from that storage
	- allocate virtual disks from the available space you have in that pool
	- these can be standalone virtual disks, they can also be mirrored or striped arrays!
	- you can also build hot spares into these virtual drive arrays
	- so if a mirrored array loses a drive, the hot spare is immediately available to act as a replacement drive
	- after which you can immediately resynchronize that data and maintain redundancy

#aplus #core2 **1.5** *Given a scenario, use Microsoft operating system features and tools.* 
