> 1.8 Given a scenario, configure Microsoft Windows networking on a client/desktop.

# Mapping drives

- to connect to a remote share, go to Explorer > This PC > Map Network Drive
- in the dialog box, select the drive letter to use to reference the share once you make the connection
- then specify the share's location, with the name of the server/device followed by the name of the share: `\\sg-server\mission-reports`
- below that are two checkboxes, the first one to reconnect to the share automatically when you sign in
- and the second one to connect using different credentials from the ones you use to sign in to your computer
- to connect to the share from the command line, see the page on [`net`](17.%20net.md)
	- `net use e: \\sg-server\mission-reports`