# `services.msc`
(part of the *administrative* tools category)

- Services lets you see the dependency tree of services
- alternatively, Control Panel > Administrative Tools > Services
- for when you're troubleshooting the startup process or controlling background apps
- if you disable the Print Spooler service you'll disable the Fax service
- again just type print and it'll highlight the print spooler service, double click it 
- from there you can click the dependencies tab to see that the print spooler relies on HTTP and RPC and is relied on by Fax

- if you have startup problems, this is your go to because it may be related to some running services
- services are background processes and not like the traditional apps you interact with directly
- services such as file indexing, anti-virus, network browsing will start automatically on startup
- `net start` and `net stop` 
- the utility lists services with their names on the left, followed by the description column, then status (running or not) on the right
- to jump to the print spooler service for example, just start typing *pri-*
- right click a service and select properties
- from here you can start it, stop it, change how it logs on to the network, how it recovers after a problem the first time, the second time, and subsequent times
- it can recover by restarting, running a program, restarting the computer

#aplus #core2 **1.5** *Given a scenario, use Microsoft operating system features and tools.* 
