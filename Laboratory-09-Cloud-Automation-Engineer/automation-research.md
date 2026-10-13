# Automation Research

## Bash Script
A Bash script is a text file that holds a series of Linux commands which the shell runs in order from top to bottom. It saves time because the whole routine can be run again with a single command. The first line, `#!/bin/bash` (the shebang), tells the system which program, in this case Bash, should read and execute the file.

## Variables
A variable is a named container for a value, like a folder path stored in `$BACKUP_DIR`. Using one means the path is written once and referenced wherever it is needed, instead of being retyped in many places. This lowers the chance of typos, and changing the path later only requires editing a single line.

## Cron Job
A cron job is a scheduled task that the Linux cron service runs by itself at the time written in the crontab. It runs in the background, so nobody has to log in or press anything. This matters in cloud operations because routine work like backups and cleanups must happen on time, every time, and cannot depend on someone remembering.
