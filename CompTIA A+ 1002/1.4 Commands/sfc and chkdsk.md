> 1.4 Given a scenario, use appropriate Microsoft command line tools. 

# `sfc` and `chkdsk`

- `sfc` (System File Checker) checks the integrity of core operating system files and repairs any damage, e.g. if you just performed an update
- `/SCANNOW` option scans the integrity of all protected system files and repairs files with problems when possible
- `/VERIFYONLY` only checks the integrity
- `/SCANFILE` checks and repairs a specific file
- `/VERIFYFILE` checks a specific file
- `/OFFBOOTDIR` is for offline repair; specify the location of the offline boot directory
- `/OFFWINDIR` lets you specify the location of an offline Windows directory 
- `/OFFLOGFILE` lets you enable logging by specifying a log file path
- oh wow the options are case insensitive, you can type `/scannow`

- `chkdsk` 
- `/f` fixes logical file system errors on disk
- `/r` locates bad sectors and recovers readable information which implies `/f` and first performs that
- if the volume is locked then run during startup
- or you can run and it'll ask if you want to run it during the next bootup since the volume is locked when in use