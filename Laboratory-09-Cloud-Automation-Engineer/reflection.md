# Mission Reflection

## 1. Why is automation critical when managing hundreds of cloud servers?
Doing tasks by hand on hundreds of servers is slow and full of chances for mistakes. Automation lets one script perform the same job on every machine in exactly the same way. It also means important routine work, like backups, does not depend on someone remembering to do it.

## 2. What are the potential dangers of automation?
Automation makes mistakes as fast as it makes progress. A destructive typo in a script scheduled on 1,000 servers, such as deleting the wrong folder, would run everywhere at once and could wipe out data before anyone notices. To lower this risk, scripts should be tested on a single server first, released in small batches, and backed by good backups.

## 3. How did writing a Bash script differ from creating a Docker Compose YAML file?
In a Bash script, I wrote the exact steps the computer should follow, one after another. In a Docker Compose YAML file, I described the setup I wanted, and Docker worked out how to build it. Bash felt more hands-on and flexible, while Compose felt more organized and easier to read at a glance.

## 4. How has my understanding of Cloud Computing transformed this semester?
At the start, in Laboratory 1, cloud computing felt like a general idea about using servers over the internet. By Laboratory 9, I understood it as a set of practical skills: building infrastructure, deploying applications, managing operations, securing systems, and automating tasks. I now see the cloud as something I can actually operate and not just define.

## 5. Which role did I enjoy the most and why?
I enjoyed the Cloud Automation Engineer role the most because the result was immediate and easy to see. A short script and a single cron line replaced a manual task completely. It showed me how a small piece of code can prevent a real problem like lost customer files.
