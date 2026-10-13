# Backup Script Guide

## Purpose
The backup script compresses the `app-data` directory into a `.tar.gz` archive. Each backup filename contains a timestamp to help distinguish backups created at different times.

## Full Bash Script

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

The command `chmod +x backup.sh` adds executable permission to the script. This allows the user to run it directly using `./backup.sh`, provided the user also has the required access permissions.

## Cron Schedule

Cron expression:

```cron
0 2 * * * /root/backup.sh
```

The five time fields mean:

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The command `/root/backup.sh` is the script that Cron runs. The schedule runs daily at 2:00 AM, using the system's time zone.

## 5. Verification
The command `ls -l backups/` lists the generated backup archive. The command `tar -tzf backups/backup_FILENAME.tar.gz` can be used to inspect the archive contents after replacing the example filename with the actual filenam
