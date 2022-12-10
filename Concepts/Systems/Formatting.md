# File system types/formatting

- the OS categorizes files via a file system
- a *full format* will write the entire drive with zeroes and check if data can be read and written to every sector
- a *quick format* just creates a new file table and doesn't erase any data that may have existed or check if 100% of the drive works
- run `diskpart` for a full format
- *FAT* (File Allocation Table) is old
- *FAT32* is newer 
	- 2 TB volume size limit
	- 4 GB file size limit
- *ExFAT* (Extended FAT) is even newer
	- made for flash drives
	- files larger than 4 GB
- *NTFS* (NT File System) 
	- bigger size limits
	- quotas, encryption, compression, oh my!
	- all the file types so far by the way are recognized by Windows
- *CDFS* (Compact Disk File System)
	- widely recognized—you can use the same CD or DVD-ROM drive on any operating system and be able to read the data
- *NFS* (Network File System)
	- for storing and accessing storage devices across a network
	- the OS just looks like a local drive on the local computer
- *ext3*, *ext4* 
	- 3rd and 4th extended file system
	- Linux and Android
- *HFS* (Hierarchical File System) AKA *macOS Extended*
	- replaced by *APFS* with High Sierra

#aplus #core2 **1.3** *Summarize general OS installation considerations and upgrade methods.* 
