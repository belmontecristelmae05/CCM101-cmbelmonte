# Backup Script Guide

## Full Backup Script

The following script creates a compressed backup of the `app-data` directory. It uses a timestamp in the filename to identify when each backup was created.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## File Permissions

The command `chmod +x backup.sh` adds executable permission to the `backup.sh` file. This allows Linux to run the script using `./backup.sh` instead of requiring the user to invoke Bash manually.

## Cron Job Configuration

The following Cron expression schedules the backup script to run every day at 2:00 AM.

```cron
0 2 * * * /root/backup.sh
```

### Explanation of the Five Time Fields

| Time Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Runs at minute zero. |
| Hour | `2` | Runs at 2 AM. |
| Day of Month | `*` | Runs on every day of the month. |
| Month | `*` | Runs during every month. |
| Day of Week | `*` | Runs on every day of the week. |

The five time fields determine when the scheduled task executes. The `/root/backup.sh` portion specifies the location of the script that Cron runs.

## Backup Verification

The command below displays the backup files created by the script.

```bash
ls -l backups/
```

To check the contents of a compressed backup, use:

```bash
tar -tzf backups/*.tar.gz
```

The archive should contain `app-data/data.txt`, confirming that the test data was included in the backup.


