# Laboratory 08: The Cloud Security Engineer

## Mission Overview

In this laboratory, I took on the role of a Cloud Security Engineer at CloudNova Technologies. My mission was to deploy an Nginx web server inside a Docker container and secure the Ubuntu server using the Uncomplicated Firewall (UFW).

I configured a Default Deny incoming policy and allowed only the necessary network traffic, including SSH for remote administration and TCP port 8080 for web application access. This activity helped me understand the importance of reducing the attack surface and applying the Principle of Least Privilege (PoLP) to improve server security.

## Objectives

- Understand the attack surface and the Principle of Least Privilege (PoLP).
- Deploy an Nginx web server using Docker.
- Verify that the web server is running and accessible using cURL.
- Inspect running containers and identify exposed network ports.
- Configure UFW with a Default Deny incoming policy.
- Allow SSH and TCP port 8080 while restricting unnecessary incoming connections.
- Verify firewall rules and confirm the firewall configuration.
- Document the laboratory activities for my GitHub Cloud Computing Portfolio.

## Commands Executed

### 1. Deploy the Nginx Web Server

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
```

### 2. Verify the Running Container

```bash
docker ps
```

### 3. Test Web Server Connectivity

```bash
curl http://localhost:8080
```

### 4. Allow SSH Connections

```bash
sudo ufw allow ssh
```

### 5. Configure Default Firewall Policies

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

### 6. Enable the Firewall

```bash
sudo ufw enable
```

### 7. Allow Web Application Traffic

```bash
sudo ufw allow 8080/tcp
```

### 8. Verify Firewall Rules

```bash
sudo ufw status verbose
sudo ufw status numbered
```

## Skills Learned

- Deploying and managing an Nginx web server using Docker.
- Mapping host ports to container ports.
- Testing web server connectivity using cURL.
- Configuring UFW on an Ubuntu Linux server.
- Implementing a Default Deny incoming firewall policy.
- Managing SSH and TCP port 8080 access.
- Applying the Principle of Least Privilege (PoLP).
- Reducing the attack surface by restricting unnecessary network access.
- Verifying firewall configurations and documenting technical procedures.
- Strengthening Linux administration and cloud security skills.

