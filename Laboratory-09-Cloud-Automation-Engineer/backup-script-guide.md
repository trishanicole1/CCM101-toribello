# Backup Script Guide

This document explains the automated backup setup built for CloudNova Technologies, so the client's IT team can understand, maintain, and reuse it.

## 1. The Backup Script (`backup.sh`)

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. What `chmod +x` Did

When the script was first created, Linux did not allow it to run, and `./backup.sh` returned "Permission denied". Running `chmod +x backup.sh` added the execute permission (`x`) to the file. After this, the script could be run as a program.

## 3. The Cron Expression

```
0 2 * * * /root/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | Runs at the start of the hour (minute 0) |
| Hour | 2 | Runs at 2 AM (24-hour clock) |
| Day of Month | * | Runs on every day of the month |
| Month | * | Runs in every month |
| Day of Week | * | Runs on every day of the week |

In short, cron runs `/root/backup.sh` every night at 2:00 AM, with no one needing to start it manually.
