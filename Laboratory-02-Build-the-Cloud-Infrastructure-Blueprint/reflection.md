
Mission Reflection

1. Which cloud infrastructure component do you think is the most important? Why?

I believe compute is the most important cloud infrastructure component because it provides the processing power needed to run applications, execute commands, process information, and respond to user requests. Compute resources mainly include the CPU and RAM, which work together to perform the operations required by applications and services. Without sufficient compute resources, other infrastructure components such as storage and networking would not be able to provide useful services to users. Storage is important because it keeps data, while networking allows different systems to communicate, but compute is responsible for processing the data and running the applications that use those resources.

During this laboratory activity, I learned that the KillerCoda server itself can be considered a compute resource. By using the lscpu and free -h commands, I was able to identify the server's CPU and memory resources. The server had one logical CPU and 1.9 GiB of RAM, showing how even a small virtual machine can provide the basic resources needed to run a Linux environment.

However, I also realized that cloud infrastructure components cannot work effectively in isolation. Compute depends on storage to access important files and data, while networking allows applications and users to communicate with the server. Because of this, I consider compute the most important component for processing workloads, but all cloud infrastructure components must work together to create a functional and reliable cloud environment.

2. How does Linux support cloud computing?

Linux plays an important role in cloud computing because it provides a stable, flexible, lightweight, and open-source operating system that can efficiently run on virtual machines, servers, and containers. Because Linux is open-source, cloud providers and organizations can customize and manage it according to their specific requirements without depending entirely on proprietary operating systems. This makes Linux a practical choice for large-scale cloud environments where organizations may need to manage hundreds or thousands of servers.

Major cloud providers such as Amazon Web Services, Microsoft Azure, and Google Cloud Platform provide many Linux-based virtual machine options. Linux is also widely used for containerized applications because of its strong support for virtualization, networking, security, and automation. Cloud administrators can use Linux command-line tools and scripting to perform tasks quickly and consistently across multiple servers.

During this laboratory activity, I experienced how useful Linux can be for cloud infrastructure investigation. I used commands such as lscpu to identify the CPU model and number of cores, free -h to check memory usage, df -h to examine disk capacity, uname -r to check the kernel version, and ip a to inspect network interfaces and IP addresses. These commands allowed me to gather important information without needing a graphical interface.

Linux also supports automation, which is important when managing cloud infrastructure at scale. Overall, Linux provides the flexibility, reliability, and powerful administrative tools needed to operate modern cloud environments efficiently.

3. Why is technical documentation important before deploying infrastructure?

Technical documentation is important before deploying infrastructure because it provides a clear record of the resources, configurations, requirements, and decisions involved in a project. Before making changes to a cloud environment, engineers need to understand what resources already exist and how those resources are connected. Without proper documentation, an organization may accidentally change an important configuration, create inconsistent deployments, or have difficulty identifying the cause of technical problems.

During this laboratory activity, documentation helped organize the information gathered from the Linux server. Commands such as lscpu, free -h, df -h, and ip a provided information about compute, memory, storage, and networking resources. Recording these results made it easier to understand the server's infrastructure and relate the information to cloud computing concepts.

Technical documentation is also valuable for teamwork. In a professional environment, multiple engineers may work on the same infrastructure. Clear documentation allows team members to understand the current configuration without having to investigate everything again. It also helps new team members become familiar with the project more quickly.

Documentation is especially useful during troubleshooting and maintenance. If a problem occurs after deployment, engineers can review the documented configuration and compare it with the current environment. This can help identify changes that may have caused the problem. Good documentation also supports future improvements because engineers can use existing information when planning upgrades, migrations, or scaling activities.

Through this laboratory, I learned that technical documentation is not simply a requirement for submitting a project. It is an important part of professional infrastructure management because it improves communication, consistency, troubleshooting, and long-term maintainability.

4. What new skills did you learn during this laboratory activity?

During this laboratory activity, I developed several new technical skills related to Linux administration, cloud infrastructure, documentation, and Git. One of the most important skills I learned was how to investigate a Linux server using command-line tools. Instead of relying on a graphical interface, I used commands such as lscpu, free -h, df -h, uname -r, hostname, and ip a to gather information about the server.

I learned how to identify important system resources, including the CPU, RAM, disk capacity, mounted filesystems, operating system, kernel version, hostname, and network interfaces. I also learned how these Linux resources relate to cloud infrastructure concepts. For example, the CPU and RAM represent compute resources, disk partitions represent storage, and network interfaces represent networking resources.

Another important skill I developed was comparing services offered by major cloud providers. I researched AWS, Microsoft Azure, and Google Cloud Platform and identified equivalent services for compute, storage, networking, and identity and access management. This helped me understand that different cloud providers may use different product names while providing similar fundamental capabilities.

I also improved my Git and GitHub skills throughout the laboratory. I learned how to configure my Git username and email, add files to the staging area, create commits with meaningful messages, and push changes to a remote repository. I also encountered authentication and session-related issues that required troubleshooting.

Finally, I improved my technical writing and documentation skills by organizing information into Markdown files. Overall, this activity helped me connect theoretical cloud computing concepts with practical Linux administration and version-control skills that can be useful in future cloud and infrastructure projects.

5. How has your GitHub portfolio improved after completing this mission?

My GitHub portfolio has improved significantly after completing this laboratory because it now demonstrates practical cloud computing knowledge rather than only theoretical understanding. The project contains organized documentation that shows how I investigated a Linux server, identified its infrastructure components, compared major cloud providers, and reflected on what I learned throughout the activity.

One of the most valuable improvements is the inclusion of a detailed infrastructure report. This report documents the operating system, kernel version, CPU model, number of CPU cores, available RAM, disk capacity, mounted filesystems, hostname, and network interfaces. These details demonstrate my ability to use Linux commands to investigate a real server environment and interpret the results.

The portfolio also includes documentation about cloud infrastructure components such as compute, storage, networking, and operating systems. In addition, I created a comparison of AWS, Microsoft Azure, and Google Cloud Platform. This shows that I understand how different cloud providers offer equivalent services and how organizations can choose platforms based on their specific requirements.

Another improvement is the inclusion of a cloud architecture diagram, which provides a visual representation of the infrastructure design. Combining diagrams with written documentation makes the project easier to understand and more professional.

The laboratory also gave me practical experience with Git and GitHub. I learned how to configure Git identity information, stage files, create meaningful commits, troubleshoot authentication issues, and push updates to the repository.

Overall, my GitHub portfolio now demonstrates a combination of Linux administration, cloud infrastructure knowledge, technical documentation, architecture planning, and version-control skills. This makes the portfolio more useful as evidence of my practical abilities and future growth in cloud computing.

