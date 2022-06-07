> 1.4 Given a scenario, use appropriate Microsoft command line tools. 

# `gpupdate` and `gpresult`

- `gpupdate`
	- `gpupdate /target:{computer|user} /force` forces a group policy update which is usually updated at login
	- group policy lets you manage computers in an Active Directory Domain
	- e.g. `gpupdate /target:professor /force` 

- `gpresult` 
	- `gpresult /r` shows group policy settings on the computer
	- `gpresult /user sgc/professor /v` for remote devices 