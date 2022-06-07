> 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

# `iwconfig` and `ifconfig`

- as a sysadmin sometimes you need to look at the network configuration of a particular Linux system
- if a device has a wireless adapter card, you want to use `iwconfig` to view or modify wireless config settings
- e.g. `iwconfig eth0` outputs info on the ssid (`essid`), channel, mode, rate, etc.
- e.g. `iwconfig eth0 essid studio-wireless` modifies the `eth0` wireless adapter's ssid to be `studio-wireless` 

- `ifconfig` views and configures network information associated with a wired network interface
- e.g. `ifconfig eth0` outputs information about the IP address, subnet masking, etc. for the adapter by the name of `eth0`
- some distros have migrated away from `ifconfig` to `ip`
- e.g. `ip address` outputs all information like `ifconfig` (no arguments) does