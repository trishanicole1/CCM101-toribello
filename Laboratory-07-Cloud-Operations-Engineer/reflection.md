# Mission 7 Reflection

## 1. Why is it important to check the host server's resources even if your containers are running perfectly?

Containers share the host's CPU, RAM, and disk, so a container can look healthy while the host is running short on resources. If the host runs out of memory or disk space, every container on it can slow down, crash, or fail to save data. My server had 1.9Gi of RAM and 19G of disk, so checking them first gave me a baseline to compare against later.

## 2. If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem?

I would run docker logs on the application's container and look at the entries made when the user tried to log in. A 401 or 403 status points to wrong credentials or blocked access, while a 500 means the server itself failed. The error messages would show the real cause, so I could fix it instead of guessing.

## 3. What is the difference between monitoring logs (Checkpoint 4) and monitoring metrics (Checkpoint 5)?

Logs are records of individual events, like my 404 request to /hidden-admin-page, so they tell me what happened and when. Metrics are numbers measured over time, like the CPU and memory values shown by docker stats, so they tell me how the system is performing. Logs explain specific problems, while metrics show trends and overload.

## 4. How do large enterprise companies monitor thousands of containers at the same time?

Companies cannot check containers one by one, so they use monitoring tools. Prometheus automatically collects and stores metrics from many containers, and Grafana turns that data into dashboards and sends alerts when a value passes a limit. This gives the operations team a single view of thousands of containers.

## 5. How has your ability to troubleshoot Linux environments improved?

Before this lab, I only knew basic commands. Now I can check memory with free -h, check disk space with df -h, read application logs with docker logs, and watch live usage with docker stats. I also learned to rely on logs and metrics as evidence instead of guessing when something goes wrong.
