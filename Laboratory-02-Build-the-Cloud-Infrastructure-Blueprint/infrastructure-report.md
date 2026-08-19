Infrastructure Report

Checkpoint 2 – Investigate the Cloud Server

Operating System

Command used: cat /etc/os-release

Result: Ubuntu 24.04.4 LTS (Noble Numbat)

Kernel Version

Command used: uname -r

Result: 6.8.0-136-generic

CPU Model

Command used: lscpu

Result: Intel Xeon E312xx (Sandy Bridge, IBRS update)

Number of CPU Cores

Command used: lscpu

Result: 1 CPU, 1 core per socket, 1 thread per core, for a total of 1 logical CPU.

Total RAM

Command used: free -h

Result: 1.9 GiB total RAM, with 413 MiB used, 831 MiB free, and 1.5 GiB available.

Disk Capacity

Command used: df -h

| Filesystem | Size | Used | Avail | Use% | Mounted on |
| ---------- | ---: | ---: | ----: | ---: | ---------- |
| /dev/vda1  |  19G | 5.4G |   13G |  30% | /          |
| /dev/vda16 | 881M | 117M |  703M |  15% | /boot      |
| /dev/vda15 | 105M | 6.2M |   99M |   6% | /boot/efi  |
| tmpfs      | 191M | 996K |  190M |   1% | /run       |
| tmpfs      | 952M |  84K |  952M |   1% | /dev/shm   |
| tmpfs      | 5.0M |    0 |  5.0M |   0% | /run/lock  |

Mounted File Systems

The cloud server has the following mounted file systems:

/ — Root filesystem containing the main operating system, with a capacity of 19G.

/boot — Boot partition with a capacity of 881M.

/boot/efi — EFI system partition with a capacity of 105M.

/run, /dev/shm, and /run/lock — Temporary in-memory filesystems using tmpfs.

Hostname

Command used: hostname

Result: ubuntu

IP Address

Command used: ip a

Result:

enp1s0 — Main network interface: 172.30.1.2/24

lo — Loopback interface: 127.0.0.1

docker0 — Docker bridge interface: 172.17.0.1
