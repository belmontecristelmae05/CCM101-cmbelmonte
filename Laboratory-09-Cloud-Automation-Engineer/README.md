# Laboratory 09 - Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating repetitive tasks using Bash scripting and Cron jobs. I created a test application directory, developed a backup script, and configured a schedule to run the script automatically every day at 2:00 AM.

## Objectives

- Understand the basic syntax of Bash scripting.
- Create and execute a backup script using Nano.
- Modify file permissions using the `chmod` command.
- Schedule automated tasks using Linux Cron.
- Document the automation process using Markdown.

## Commands Executed

- `mkdir app-data`
- `echo "This is critical client data." > app-data/data.txt`
- `nano backup.sh`
- `./backup.sh`
- `chmod +x backup.sh`
- `ls -l backups/`
- `tar -tzf backups/*.tar.gz`
- `crontab -l`
- `env EDITOR=nano crontab -e`

## Skills Learned

I learned how to write Bash scripts to automate repetitive tasks in Linux. I also learned how to create compressed backup files, give scripts executable permission using `chmod +x`, and schedule automatic tasks using Cron. This activity improved my understanding of how automation can make cloud operations easier and reduce the need for manual work.
