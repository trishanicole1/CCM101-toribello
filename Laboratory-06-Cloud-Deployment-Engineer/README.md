# Laboratory 06: Cloud Deployment Engineer

## Mission Overview

In this mission, I deployed a private cloud storage system using Nextcloud and MariaDB as a two-tier application. Instead of starting containers one by one, I wrote a `docker-compose.yml` file (Infrastructure as Code) and deployed the whole stack with a single command in a KillerCoda Ubuntu Playground.

## Objectives

- Explain the concept of a multi-tier application architecture
- Understand the purpose and structure of a `docker-compose.yml` file
- Use a Linux command-line text editor to create configuration files
- Deploy a multi-container application using Docker Compose
- Document deployment procedures and IaC principles using Markdown
- Continue expanding my GitHub Cloud Computing Portfolio

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir nextcloud-deployment` | Create the project directory |
| `cd nextcloud-deployment` | Move into the project directory |
| `cat > docker-compose.yml << 'EOF'` | Create the Compose file |
| `docker-compose up -d` | Deploy all containers in the background |
| `docker-compose ps` | Check that the containers are running |
| `docker-compose down` | Stop and remove the containers and network |
| `git add`, `git commit`, `git push` | Save and upload my work to GitHub |

## Skills Learned

- Writing a multi-container configuration in YAML
- Deploying and tearing down a stack with Docker Compose
- Understanding how services find each other by name on a shared network
- Documenting infrastructure in Markdown
