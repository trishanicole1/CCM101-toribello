# Docker Deployment Log

| Command | Explanation |
|---|---|
| docker ps | Lists all currently running containers. |
| docker stop my-nginx | Gracefully stops the running my-nginx container. |
| docker ps -a | Lists all containers, including stopped ones, to confirm my-nginx has exited. |
| docker rm my-nginx | Permanently removes the stopped container and its writable layer. |

