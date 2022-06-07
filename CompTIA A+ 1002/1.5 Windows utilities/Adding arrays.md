> 1.5 Given a scenario, use Microsoft operating system features and tools. 

# Disk Management: adding arrays

- continuing off from [Disk Management](Disk%20Management.md)
- again, mirroring and striping is only allowed in some Windows versions
- say you have two newly installed disks each with 120 GB
- right click on one of the two drives and select new mirrored volume
- the disk you right clicked will be preselected and you need to select one more, the other available one will be shown
- instead of mounting like we discussed above, this time choose *Assign the following drive letter: E* (or whatever letter)
- after that the default settings are to format the volume with NTFS and call it *New Volume*
- below those settings is a checkbox if you want to perform a quick format, meaning you don't want to identify each bad block/sector/whatever it's called
- after you finish you will see a warning: *The operation you selected will convert the selected basic disk(s) to dynamic disk(s). If you convert the disk(s) to dynamic, you will not be able to start installed operating systems from any volume on the disk(s) (except the current boot volume). Are you sure you want to continue?*
- in our case these are simple data volumes and we're not booting any operating systems so choose *Yes*
- after a little wait you will see the two disks previously called *Unallocated* turn from black to red and be renamed to *New Volume (E:)*
- you will also see *New Volume (E:)* added to the list at the top section of the utility
- to the user it's one drive, but you and I know it's two drives containing redundant info that is being mirrored by Windows