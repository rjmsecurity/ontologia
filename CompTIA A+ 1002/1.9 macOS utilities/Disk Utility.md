> 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

# Disk Utility

- "scheduled disk maintenance" for CompTIA but it's commonly manual, as-needed
- if you have drive problems, use the First Aid function 
- First Aid is similar to Windows Check Disk
- it examines your drive, makes sure all file permissions are set properly, ensures the OS can operate properly using that particular drive

- other functions include Partition, Erase, Restore, Unmount
- e.g. if you have a new drive, partition then erase (format) it

- Windows sysadmins may be familiar with building *images* to back up information and restoring from them, which you can do in macOS too with Disk Utility
- Disk Utility builds Apple's version of an image called a .dmg file (Apple Disk Image)
- you can create and mount a disk image file on any macOS system and it appears as a normal file system but it's an image file 
- you then copy files from the image
- you can also back up a large section of a drive to an image and then later use the Restore function

- in addition to images, you can also manage disks connected to your macOS (see partitioning and erasing above)
- finally, you can expand or remove information from (*shrink*?) a particular image 