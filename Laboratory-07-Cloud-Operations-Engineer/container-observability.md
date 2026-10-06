# Container Observability

## Application Logs (404 Error)
```
172.17.0.1 - - [06/Oct/2026:04:14:08 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs record every request along with its status code, so they show exactly what happened and when. This lets an engineer quickly find the failing request and its cause instead of guessing.

## Container Metrics (docker stats)

- Container: client-website
- CPU Usage: 0.00%
- Memory Usage: 2.727MiB
