# Laboratory 09 - Cloud Automation Engineer

## Mission Overview
In this mission, I took the role of a Cloud Automation Engineer at CloudNova Technologies. The client's IT staff kept forgetting to back up their application data, which once led to permanent loss of customer files. To remove this human error, I wrote a Bash script that compresses the application folder into a timestamped archive, tested it, and scheduled it with cron to run automatically every night at 2:00 AM.

## Objectives
- Understand the basic syntax of a Bash script, including variables and basic commands
- Write and save a script from the command line
- Change file permissions using `chmod`
- Understand task scheduling and the syntax of a Linux crontab
- Document automation code and cron job configurations using Markdown
- Complete the final chapter of the GitHub Cloud Computing Portfolio

## Commands Executed
```bash
# Setup and dummy data
cd ~
mkdir app-data
echo "This is critical client data." > app-data/data.txt

# Create the script
cat > ~/backup.sh
cat ~/backup.sh

# Permissions and execution
./backup.sh
chmod +x backup.sh
ls -l backup.sh
./backup.sh
ls -l backups/

# Cron scheduling
crontab -l
env EDITOR=nano crontab -e
crontab -l

# Git
git add .
git commit -m "message"
git push
```

## Skills Learned
- Writing a Bash script that uses variables and basic commands
- Compressing a directory into a `.tar.gz` file with `tar`
- Making a script executable with `chmod +x`
- Scheduling recurring tasks with cron and reading crontab syntax
- Documenting technical work in Markdown
- Managing project files with Git and GitHub
