# Laboratory 4: The Cloud-Native Engineer

## Mission Overview
This lab documents my work as part of CloudNova Technologies' Cloud-Native Engineering Team, tasked with
helping a client move away from slow, resource-heavy Virtual Machines toward lightweight, fast-deploying
Docker containers. The activity covered comparing VM and container architecture, confirming that Docker
was properly installed and running, deploying a live Nginx container, and documenting the full container
lifecycle so the client's IT team could reproduce the same setup.

## Objectives
- Explain the key differences between Virtual Machines and Containers.
- Set up and access a Docker-enabled environment through KillerCoda.
- Run core Docker CLI commands confidently.
- Pull, launch, manage, and remove a containerized Nginx application.
- Produce clear, professional Markdown documentation of the process.
- Keep building out a structured GitHub Cloud Computing portfolio.

## Docker Commands Executed

*Checkpoint 3 — Verifying Docker*
docker --version
docker info

*Checkpoint 4 — Deploying Nginx*
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080

*Checkpoint 5 — Container Lifecycle*
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx

## Skills Learned
- Verifying that Docker is installed and the daemon is actively running.
- Pulling pre-built images from Docker Hub.
- Understanding how port mapping (-p host:container) exposes a container's service to the outside world.
- Managing a container's full lifecycle, from listing and stopping to removing it entirely.
- Recognizing why containers are more resource-efficient and faster to deploy than traditional VMs.

## Challenges Encountered
The KillerCoda environment came pre-configured with Docker, so setup itself was smooth. The main
adjustment was getting used to Docker's command syntax and remembering flags like -d and -p correctly
on the first attempt, which became easier after running through the lifecycle commands a few times.
