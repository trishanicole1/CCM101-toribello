# Laboratory 10: The Enterprise Cloud Architect

*Course:* CCM101 – Cloud Computing
*Student:* Trisha Nicole M. Oribello
*Institution:* University of Eastern Pangasinan, College of Information Technology
*Client scenario:* CloudNova Technologies (CEO: Cledmar Badongen)

## Overview

This project is a secure, automated, multi-tier private cloud environment. It deploys a *WordPress + MariaDB* stack using Docker Compose (Infrastructure as Code), hardened with UFW (default deny incoming), and protected by an automated database backup script scheduled with cron.

## Chosen Stack

| Tier | Technology | Purpose |
|------|-----------|---------|
| Application | WordPress | Web application |
| Database | MariaDB 11 | Persistent data storage |
| Orchestration | Docker Compose | Defines and links the containers |
| Host OS | Ubuntu Server | Base operating system |
| Firewall | UFW | Host-based security, default deny |
| Automation | Bash + Cron | Scheduled database backups |

## Architecture

See architecture-diagram.png.

*Flow:* Host Laptop → Hypervisor → Ubuntu Server VM → UFW Firewall → Docker Network → WordPress + MariaDB → Persistent Volumes

## Repository Contents

| File | Description |
|------|-------------|
| README.md | Project overview (this file) |
| architecture-diagram.png | Network topology and architecture diagram |
| docker-compose.yml | Infrastructure as Code for the two-tier stack |
| automation-script.sh | Bash script that backs up the MariaDB database |
| setup-ufw.sh | Firewall hardening script |
| operational-manual.md | Deploy, secure, and maintain guide for the client IT team |
| final-reflection.md | Reflection on Missions 1 to 10 |
| .env.example | Template for environment variables |

## Requirements Checklist

- [x] *Requirement 1:* Architecture diagram, Ubuntu Server VM, browser access from host
- [x] *Requirement 2:* Docker and Docker Compose, two linked containers, persistent volumes
- [x] *Requirement 3:* UFW enabled, default deny, only SSH and application port allowed
- [x] *Requirement 4:* Executable Bash script and cron job
- [x] *Requirement 5:* Operational manual, raw code committed, final reflection

## Quick Start

# 1. Create the environment file (use your own strong passwords)
cp .env.example .env

# 2. Start the stack
docker compose up -d

# 3. Verify that both containers are running
docker compose ps

# 4. Open in a browser
# http://<server-ip>:8080

## Security Summary

- UFW is enabled with *default deny incoming*.
- Only SSH (22/tcp) and WordPress (8080/tcp) are allowed.
- The database container publishes no ports and is reachable only on the internal Docker network.
- Credentials are stored in .env, which is excluded from Git through .gitignore.

## Automation Summary

automation-script.sh creates a compressed dump of all databases, saves it to backups/, and deletes backups older than 7 days. Cron runs it daily at 2:00 AM.

cron
0 2 * * * /path/to/automation-script.sh

## Environment Note

The Docker stack, firewall, and automation were tested on a Killercoda Ubuntu sandbox. The hypervisor and Ubuntu Server VM design is shown in architecture-diagram.png.

## AI Usage Disclosure

I used an AI assistant (Claude) to help with the project structure and to clarify commands. I reviewed and tested the configuration and can explain each part. The final reflection reflects my own experience.
