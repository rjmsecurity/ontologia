> 1.9 Given a scenario, use features and tools of the Mac OS and Linux client/desktop operating systems. 

# Unix commands intro

- Linux distros either have Terminal, XTerm, or similar
- macOS and Linux commands are similar because Linux is modeled after Unix and macOS is derived from BSD (Berkeley Software Distribution) Unix
- since they're similar or identical we are focusing on Linux 

- `man` manual e.g. `man grep` pulls the online manual on the grep command

- `cd` change directory
- `pwd` print working directory

- `ls` list directory contents – may be color coded, e.g. blue text is a directory, white is a file
- `ls -l` for long output, which shows permissions, owner, group, size, timestamp, and name

- `ls -l | more` to pipe it to `more` so that it paginates instead of a hundred lines zipping by in a millisecond
- `more auth.log` does the same as `cat` but again with pagination
- press `q` or `Ctrl-c` to exit a paginated output

- `grep failed auth.log` to find all the lines in the `auth.log` file that match the word `failed`