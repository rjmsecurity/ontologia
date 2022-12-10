# `dd`

- going off of [Disk Utility](Disk%20Utility.md), Windows has many imaging options; Linux not so much but there are still multiple options
- `dd` is designed to convert and copy a file 

- in Linux, everything looks like a file, so you're able to back up and restore entire partitions using `dd`
- `dd if=<source file name> of=<target file name> [Options]`
- `dd if=/dev/sda of=/tmp/sda-image.img` to backup the `/dev/sda` partition

- to restore from that image, `dd if=/tmp/sda-image.img of=/dev/sda`

- 3rd-party utilities used for imaging in Linux include GNU Parted and Clonezilla
- *to image a drive* is another way to refer to imaging

#aplus #core2 **1.9** *Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems.* 
