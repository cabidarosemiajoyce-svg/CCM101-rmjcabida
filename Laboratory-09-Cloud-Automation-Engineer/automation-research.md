# Automation Research

## Bash Script
A Bash script is a text file containing commands that Linux can execute in sequence. The `#!/bin/bash` line, called the shebang, tells the system to use Bash to interpret the commands in the file.

## Variables
Variables store values, such as folder paths, that a script can reuse. For example, `$BACKUP_DIR` allows the script to refer to the backup folder without repeatedly typing its path, making the script easier to maintain.

## Cron Job
A Cron job is a scheduled task in Linux that runs a command or script at a specified time. It is useful in cloud operations because recurring tasks, such as backups, can run automatically without someone manually starting them.
