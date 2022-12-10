# copy

- `copy` copies a file or list of files from one directory to another directory in the same storage device or a different one
- `/v` verifies that new files are written correctly
- `/y` suppresses prompting to confirm if you want to overwrite an existing destination file
- `copy /y /v C:\Users\Jon\Downloads\*.mp3 C:\Users\Jon\Music\DownloadedMusic\ `

- `xcopy` copies multiple files and directories
- it's the equivalent of `cp -rf`
- `/S` copies directories and subdirectories except for empty ones
- e.g. `xcopy /s Documents e:\backups` (under backups folder which already exists)

- `robocopy` (robust copy) is a better version of xcopy
- if a file transfer is interrupted you are able to resume it—good for WANs
- `robocopy /s Documents e:\backups` 
- by the way the e: drive in Professor's case is his flash drive, I'm sure it could be anything

#aplus #core2 **1.4** *Given a scenario, use appropriate Microsoft command line tools.* 
