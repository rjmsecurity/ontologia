> 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

# Disk maintenance

- Linux doesn't require ongoing disk maintenance, a lot of the maintenance in Linux is built-in
- just have enough resources and keep enough space for your data

- if you need to perform a check of the filesystem and confirm everything works as expected: 
- `sudo touch /forcefsck` (filesystem consistency check)
- first make sure the partition is not mounted – the filesystem cannot be mounted
- it's common to perform this check during startup, before any partition is mounted into the OS
- this check is normally automatically done every x number of reboots
- maybe your system doesn't reboot often so you need to force a check
- so when you run this command, the next time you reboot your system it will perform this consistency check

- another thing is to clean up log space if you're running out of space, as log files tend to pile up
- go through `/var/log` and delete old log files