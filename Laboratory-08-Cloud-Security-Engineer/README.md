# Laboratory 8: The Cloud Security Engineer

## Mission Overview
In this mission, I acted as a Cloud Security Engineer at CloudNova Technologies. I deployed an Nginx web server in a Docker container, then secured the Ubuntu server using UFW. I set a Default Deny policy and allowed only SSH and port 8080, which are the services the client needs.

## Objectives
- Understand the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement granular port management to selectively allow SSH and HTTP traffic.
- Document firewall rules and security best practices using Markdown.
- Continue expanding my professional GitHub Cloud Computing Portfolio.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned
- Deploying a web application using a Docker container.
- Checking if a service is reachable using curl.
- Configuring UFW with a Default Deny policy.
- Allowing only specific ports (SSH and 8080) to keep the attack surface small.
- Allowing SSH before enabling the firewall to avoid getting locked out.
- Documenting work in Markdown and pushing it to GitHub.
