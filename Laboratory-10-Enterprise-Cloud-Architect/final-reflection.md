# Final Reflection: Mission 1 to Mission 10

*Student:* Trisha Nicole M. Oribello
*Course:* CCM101 – Cloud Computing

## 1. Where I Started

Before Mission 1, I had never used the Linux terminal, and I thought cloud computing only meant storing files online.

## 2. My Journey

- *Missions 1–3 (Welcome to the Cloud, Build the Cloud Infrastructure, Multi-Cloud Explorer):* I learned what cloud computing is, how cloud infrastructure is built, and how different providers compare.
- *Missions 4–6 (Cloud Native, Cloud Data, Cloud Deployment):* I learned to run Docker containers, keep data persistent with volumes, and deploy applications.
- *Missions 7–9 (Cloud Operations, Cloud Security, Cloud Automation):* I learned monitoring, firewall security, and Bash scripting with scheduled tasks.
- *Mission 10 (Enterprise Cloud Architect):* I designed and deployed a WordPress + MariaDB stack with Docker Compose, secured it with UFW (default deny), and automated database backups with a Bash script and cron.

## 3. Challenges and How I Solved Them

- *Git push confusion:* My Lab 10 folder did not appear on GitHub because Git does not track empty folders. I fixed it by adding a file, committing, and pushing. Lesson: a folder only exists in Git once it contains a tracked file.
- *Overwritten README:* I accidentally overwrote the root README.md by running my command in the wrong folder. I used git show --stat HEAD to find the problem and git checkout HEAD~1 -- README.md to restore the file. *Lesson: always check the terminal path with pwd before running commands.*
- *Docker and the firewall:* Docker publishes ports by editing iptables directly, so a UFW rule alone may not control access to a container port. I solved this by giving the database container no published ports, so only the WordPress port is reachable from outside. Lesson: test the firewall from outside instead of trusting the rules alone.

## 4. Key Lessons

1. Infrastructure as Code (docker-compose.yml) makes deployments repeatable.
2. Security must be built in from the start: default deny, with only the necessary ports open.
3. Backups and automation protect a system when something goes wrong.

## 5. How Chapters 1–9 Connect in My Final Project

Virtualization provides the Ubuntu Server foundation. Containers run the WordPress and MariaDB tiers, and persistent volumes keep the data after a reboot. UFW secures the host, while Bash and cron keep backups running without manual work.

## 6. What I Would Improve

With more time, I would add HTTPS, monitoring with alerts, and off-site backups.

## 7. Final Thoughts

I started out thinking of cloud computing as a place to store files online. Now I see it as a set of connected tools for building, securing, and automating real systems. Mission 10 showed me that I can design and deploy a complete infrastructure without step-by-step instructions. The part I am most proud of is that the system is secure and can back itself up.
