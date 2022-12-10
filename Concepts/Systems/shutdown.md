# `shutdown`

- since the Windows command is so similar I moved it in here: this is how to shut down your Mac or PC!
- maybe you're troubleshooting a remote computer and can't touch the power button

- in Linux it requires elevated rights, so `sudo shutdown 2` this will shut down the computer in two minutes
- `sudo shutdown -r 2` the `r` flag means you want to also reboot after the shutdown two minutes from now
- `Ctrl-C` to cancel the shutdown or `shutdown -c` if your particular distro returns you to the prompt after you execute `shutdown`

- Windows: `shutdown /s /t 60`  will shutdown (`/s`) after 60 seconds pass (`/t 60`) 
- `shutdown /r /t 60` will not only shutdown after 60 seconds but also restart
- `shutdown /a` to abort the shutdown

#aplus #core2 **1.4** *Given a scenario, use appropriate Microsoft command line tools.* 
#aplus #core2 **1.9** *Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems.* 
