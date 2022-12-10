# `dism`

- `dism` (Deployment Image Servicing and Management tool) lets you manage WIM (Windows Imaging Format) formatted files
- make changes, view files, and perform other functions associated with these images
- `dism`  alone will show options 
- `dism /Get-WIMInfo /WimFile:d:\sources\boot.wim` will pull WIM information from a Windows image file located at `d:\sources\boot.wim`
- the information includes indices, names like PE x64 and Setup x64 which is the image file you used to set up Windows
- is `dism` what Messer meant in [Disk Utility](Disk%20Utility.md) when he said Windows has many options for imaging a Windows drive and restoring it? 

#aplus #core2 **1.4** *Given a scenario, use appropriate Microsoft command line tools.* 
