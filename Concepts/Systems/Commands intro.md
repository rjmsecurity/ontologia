# Commands intro
- `ipconfig` – computer's IP, ping your local router/default gateway and get its info, the subnet mask, ethernet adapter
- `ipconfig /all` – shows you all information including DNS server info, DHCP server info

- `taskkill` and `tasklist` are command line alternatives to the task manager
	- tasklist displays a list of currently running processes
	- local and remote
	- e.g. `TASKKILL /IM notepad.exe`
	- you can also terminate the above task by its process ID or PID: `TASKKILL -PID 1234 /T`
	- taskkill terminates task by process id (PID)

- some commands are available with standard privileges and others with administrative privileges only
- for the latter, you must be a member of the Administrators group
- right click the cmd prompt and select run as administrator
- alternatively you can enter a command and ctrl+shift+enter to run as administrator

#aplus #core2 **1.4** *Given a scenario, use appropriate Microsoft command line tools.* 
