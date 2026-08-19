
Laboratory 02 – Build the Cloud Infrastructure Blueprint

Mission Overview

This laboratory activity simulates the planning phase of a cloud deployment for a fictional company, CloudNova Technologies. Using a Linux server provisioned through the KillerCoda Playground, I investigated the underlying infrastructure, identified its major components, compared how the three major public cloud providers offer equivalent services, and designed a simple cloud architecture diagram. All findings are documented as part of a Cloud Infrastructure Assessment Report.

Objectives

* Explain the major components of cloud infrastructure.
* Investigate the hardware and software resources available in a Linux environment.
* Differentiate compute, storage, networking, and identity resources.
* Interpret the relationship between cloud infrastructure components.
* Create professional technical documentation using Markdown.
* Continue building a structured GitHub Cloud Computing Portfolio.

Cloud Infrastructure Components

Compute

Compute refers to the processing power provided by the CPU and RAM that allows applications and workloads to run. It was investigated using the lscpu and free -h commands on the KillerCoda server.

Storage

Storage refers to the resources used to store data either temporarily or persistently. It was investigated using the df -h command, which displayed partitions such as /dev/vda1 mounted at /.

Networking

Networking enables communication between systems, servers, users, and the internet. It was investigated using the ip a command, which revealed the server's private IP address and available network interfaces.

Operating System

The operating system manages hardware resources and provides the environment required to run applications and services. The server runs Ubuntu 24.04.4 LTS, as confirmed using the cat /etc/os-release command.

Full details are documented in cloud-components.md and infrastructure-report.md.

Tools Used

* KillerCoda Playground for the Linux terminal and server environment
* Git and GitHub for version control and portfolio hosting
* Markdown for technical documentation
* Draw.io for creating the cloud architecture diagram

Linux Commands Executed

| Command             | Purpose                                     |
| ------------------- | ------------------------------------------- |
| cat /etc/os-release | Identify the operating system               |
| uname -r            | Check the kernel version                    |
| lscpu               | View the CPU model and core count           |
| free -h             | Check the total RAM                         |
| df -h               | Check disk capacity and mounted filesystems |
| hostname            | Get the server hostname                     |
| ip a                | View network interfaces and IP addresses    |

Skills Learned

* How to inspect a Linux server's hardware and software resources using command-line tools.
* How to relate Linux system components such as CPU, RAM, disk, and network interfaces to cloud infrastructure concepts.
* How to compare equivalent services across AWS, Microsoft Azure, and Google Cloud Platform.
* How to design a basic cloud architecture diagram and prepare it for documentation.
* How to create clear and organized technical documentation using Markdown.
* How to use Git and GitHub to manage and maintain a technical portfolio.

Challenges Encountered

* Initially, I had difficulty committing changes to Git because the Git user identity was not configured. The user.name and user.email settings had to be configured again after the KillerCoda session reset.
* I needed to switch from password-based GitHub authentication to a Personal Access Token because GitHub no longer accepts regular account passwords for terminal-based Git operations.
* I had to carefully check git status and git log to confirm that changes were properly staged and committed. A missing commit step caused some files to remain unpushed until the issue was identified and corrected.

