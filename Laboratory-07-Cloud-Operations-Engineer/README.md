# Laboratory 07 – Cloud Operations Engineer

## Mission Overview
In this mission, I acted as a Cloud Operations Engineer at CloudNova Technologies. I checked the health of the host server, deployed an Nginx container, generated web traffic, and used logs and metrics to confirm that the application was healthy and ready for a surge in users.

## Objectives
- Monitor host CPU, memory, and disk capacity using native Linux commands
- Deploy a web container and track its real-time performance using Docker metrics
- Generate web traffic and extract application access logs for analysis
- Translate raw performance data into a readable technical report using Markdown
- Continue expanding my GitHub Cloud Computing Portfolio

## Monitoring Commands Executed
| Command | Purpose |
|---|---|
| `free -h` | Check memory (RAM) usage |
| `df -h` | Check disk storage capacity |
| `top` | View running processes and CPU load |
| `docker run -d --name client-website -p 8080:80 nginx` | Deploy the Nginx web server |
| `curl http://localhost:8080` | Simulate user traffic (HTTP 200) |
| `curl http://localhost:8080/hidden-admin-page` | Trigger a 404 error |
| `docker logs client-website` | View application access logs |
| `docker stats` | View live container CPU, memory, and network usage |

## Skills Learned
- Establishing a host performance baseline with Linux CLI tools
- Deploying and naming Docker containers
- Generating test traffic with curl
- Reading HTTP status codes (200 and 404) in application logs
- Reading real-time container metrics with docker stats
- Documenting results in Markdown and pushing them to GitHub
