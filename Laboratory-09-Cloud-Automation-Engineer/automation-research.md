# Automation Research

## Bash Script

A Bash script is a text file that groups Linux commands together so they can be performed automatically in a particular order. The `#!/bin/bash` line at the beginning identifies Bash as the program that should interpret and execute the commands in the file.

## Variables

Variables act as named containers for information that a script needs to use, such as the location of files or folders. Using a variable like `$BACKUP_DIR` makes the script easier to maintain because the stored value can be changed in one place without editing every command that refers to it.

## Cron Job

A cron job is a Linux feature that allows a command or script to run according to a schedule set by the user. Cloud administrators use cron jobs to handle regular activities, such as creating backups at night, even when nobody is available to start the process manually.
