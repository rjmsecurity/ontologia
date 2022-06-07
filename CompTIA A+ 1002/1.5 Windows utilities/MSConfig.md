> 1.5 Given a scenario, use Microsoft operating system features and tools. 

# MSConfig (System Configuration)

- `msconfig` or Control Panel > Administrative Tools
- manage the boot process, configure how Windows starts up, choose what programs and services run during boot
- the General tab lets you choose what part of Windows is going to start up during boot
	- *normal* means everything loads as it normally does
	- *diagnostic startup* is like safe mode, it only load basic devices and services
	- *selective startup* means you choose if to load system services, startup items, and/or original boot configurations
- the Boot tab is where you go if you're troubleshooting a Windows boot problem
	- if you have multiple operating systems, you can choose which one to boot to here
	- advanced options lets you select how many processors will start during boot, max memory, and other debug settings
	- boot options lets you force Windows to start into safe boot, boot without GUI, create a boot log when the system starts, and has other diagnostics
- the Services tab lets you choose which services you want to start during boot and which ones you don't
	- because a problem with a service during boot can affect the entire boot process
	- so I guess this is a second `services.msc` for redundancy thx microsoft
	- simply checkmark services, I guess it's better than services.msc in that way, it's focused on boot up
	- it may take trial and error to determine faulty service!
- the Startup tab is like the above tab but for apps you want to run on boot
	- same drill, checkmark apps and also it may take trial and error to find an app causing boot up problems
	- if you're running 8/8.1/10 then this tab is blank and redirects you to the task manager
- the Tools tab lists helpful utilities and tools I guess because it's "easier" to launch than from the command prompt or Windows menus
	- e.g. change UAC settings, computer management, event viewer