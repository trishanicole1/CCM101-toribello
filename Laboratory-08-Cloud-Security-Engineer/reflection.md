# Mission Reflection

## 1. How does a host-based firewall protect a server even if the physical network perimeter is breached?

A host-based firewall adds another layer of security by controlling incoming and outgoing network traffic directly on the server. Even if an attacker bypasses the network firewall, the host-based firewall can still block unauthorized connections based on its rules. This helps protect the server from potential attacks.

## 2. Why is managing open network ports critical to reducing a server's attack surface?

Managing open ports is important because each accessible port may expose a service that attackers can target. Closing unnecessary ports reduces the number of possible entry points into the server. Only the ports required for specific services, such as SSH for remote administration, should be allowed.

## 3. Why is it dangerous to leave a database port (like 3306 for MySQL) open to the public internet?

Leaving MySQL port 3306 open to the public internet allows attackers to attempt password guessing and exploit vulnerabilities in the database service. If they gain access, sensitive information could be stolen, modified, or deleted. To reduce this risk, database access should be restricted to trusted systems and private networks whenever possible.

## 4. How did completing this mission change your perspective on how easily a server can be compromised?

This mission helped me understand that servers can face security risks when unnecessary ports and services are exposed. I also learned that simple security measures, such as configuring firewall rules and allowing only required connections, can greatly improve server protection. It showed me that proper security configuration is an important part of managing a cloud server.

## 5. How does your GitHub portfolio currently look with eight completed missions?

My GitHub portfolio contains my laboratory activities and documentation, showing the progress I have made in learning cloud computing and server security. Completing these missions has helped me practice technical skills and organize my work in a repository. As I continue adding documentation and screenshots, my portfolio can become a useful record of my learning and practical experience.
