> 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

# `chmod`

- change the *mode*, or permissions, of a file system *object*, or file
- permissions are set for the file owner (u), the group (g), others (o), or for all three at once (a)
- `chmod a-w first.txt` means all users (`a`) are no longer allowed (`-`) to write to the file (`w`)
- `chmod u+x script.sh` means the owner (`u`) is now allowed (`+`) to execute the file (`x`)
- also from experience I know `chmod a+x` is the same as `chmod +x` 

- `chmod 744 script.sh` sets the owner's permissions to `7`, the group associated with the file to `4`, and everyone else not part of the user or group to `4`
\# | Permission | r w x
-- | - | -
0 | none | - - - 
1 | execute only | - - x
2 | write only | - w - 
3 | write and execute | - w x
4 | read only | r - - 
5 | read and execute | r - x
6 | read and write | r w -
7 | read, write, and execute | r w x
- as you can see it's like binary 
- `-rwxr--r-- 1 professor staff 8980 Aug 8 10:27 script.sh` this output translates back to `744` 