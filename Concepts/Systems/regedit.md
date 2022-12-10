# `regedit`
(regedit is part of the *system utilities* category)
-> the *run line* is the name for the search bar in the start menu where you can type the name of an app to run it
-> you can also use the command line to start utilities
-> `cmd` type this in the run line to bring up the command line

- the Windows Registry is a large, hierarchical database used by almost every service and app
- installed video game's settings, Notepad font, kernel, drivers, SAM security account manager, user interface
- best practice is to back up a portion of the registry called a *hive* before you make changes to it
- on the left are HKEYs (handle to registry key): classes root, current user, local machine, users, and current config
- HKEY_LOCAL_MACHINE > SOFTWARE > Microsoft > (just start typing notepad and it'll highlight) Notepad > DefaultFonts
- on the right the columns are registry names, types, and data
- double click the Notepad IfFaceName to change that value data
- again, before doing so, while the DefaultFonts hive is selected, go to File > Export and give it a name
- double clicking that .reg file will bring back the settings you saved

#aplus #core2 **1.5** *Given a scenario, use Microsoft operating system features and tools.* 
