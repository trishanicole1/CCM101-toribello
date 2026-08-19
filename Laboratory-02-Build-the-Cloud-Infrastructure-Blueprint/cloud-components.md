
Cloud Infrastructure Components

Compute Resources

Purpose: Compute resources refer to the processing power (CPU) and memory (RAM) that execute tasks, run applications, and process data.

Importance in Cloud Computing: Compute is the core engine of any cloud service. It allows virtual machines, containers, and applications to run. Cloud providers allow users to scale compute resources up or down based on demand, providing greater flexibility than fixed physical hardware.

Relation to KillerCoda Linux Environment: The KillerCoda server itself is a compute resource. It is a virtual machine running with 1 vCPU (Intel Xeon E312xx) and 1.9 GiB of RAM, as shown by the lscpu and free -h commands. This is similar to how a cloud provider such as AWS provisions a virtual instance for a user.

Storage Resources

Purpose: Storage resources are used to store data, files, and system information, either temporarily through RAM or persistently through disk storage.

Importance in Cloud Computing: Reliable and scalable storage allows cloud applications to save and retrieve data when needed. It also ensures that important data persists even when compute instances are stopped or restarted.

Relation to KillerCoda Linux Environment: The df -h command showed the server's disk partitions, including /dev/vda1 with 19G of storage mounted at /. The /boot and /boot/efi partitions are also used for system boot files. These partitions serve as the persistent storage layer of the virtual server, similar to block storage services such as AWS EBS attached to virtual machines.

Networking Resources

Purpose: Networking resources allow servers to communicate with each other, users, and the internet through IP addresses, network interfaces, and routing.

Importance in Cloud Computing: Networking connects compute and storage resources and allows services to communicate with users and other systems. Without networking, cloud resources would be isolated and inaccessible.

Relation to KillerCoda Linux Environment: The ip a command revealed several network interfaces. The enp1s0 interface has the private IP address 172.30.1.2/24 and is used for network communication. The lo interface is the loopback interface with the address 127.0.0.1, while docker0 with the address 172.17.0.1 is used for Docker container networking. This setup is similar to how cloud virtual machines use private or public IP addresses and virtual network interfaces.

Operating System

Purpose: The operating system manages hardware resources, runs processes, and provides the environment in which applications and services operate.

Importance in Cloud Computing: The operating system serves as the foundation for cloud services. It determines application compatibility, security updates, available tools, and how efficiently system resources are managed.

Relation to KillerCoda Linux Environment: The server runs Ubuntu 24.04.4 LTS with kernel version 6.8.0-136-generic, as confirmed by the cat /etc/os-release and uname -r commands. Linux is widely used in cloud environments because it is open-source, lightweight, stable, and supported by major cloud providers such as AWS, Azure, and Google Cloud.

