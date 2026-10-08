# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

In this laboratory activity, I practiced monitoring system resources and managing a Docker container. I checked memory and disk usage, deployed an Nginx web server, tested HTTP requests, inspected container logs, and monitored container performance.

## Objectives

- Monitor system memory and disk usage.
- Observe CPU activity and running processes.
- Deploy an Nginx container using Docker.
- Test successful and unsuccessful HTTP requests.
- Analyze Docker container logs.
- Monitor container resource usage.
- Document the results using screenshots.

## Checkpoint 2: System Resource Monitoring

I used Linux commands to check memory usage, disk space, and running processes.

Commands used:

- `free -h`
- `df -h /`
- `top`

### Memory Check

The `free -h` command displays the system's memory usage.

![Memory Check](screenshots/memory-check.png)

### Disk Check

The `df -h /` command displays the disk space used by the root filesystem.

![Disk Check](screenshots/disk-check.png)

## Checkpoint 3: Deploying Nginx

I deployed an Nginx container using Docker.

Command used:

`docker run -d --name clientwebsite -p 8080:80 nginx`

I verified the container using `docker ps`.

The container was named `clientwebsite`, and port 8080 on the host was mapped to port 80 inside the container.

### Nginx Installation Screenshot

![Nginx Installation](screenshots/install-nginx.png)

## Checkpoint 4: Simulating Website Requests

I used the `curl` command to test the Nginx web server.

Commands used:

- `curl http://localhost:8080`
- `curl -I http://localhost:8080`
- `curl http://localhost:8080/hidden-admin-page`

The root page returned HTTP 200 OK, indicating a successful response. The nonexistent page returned HTTP 404 Not Found.

### Simulation 1: Successful Request

![Simulation 1](screenshots/simulation1.png)

### Simulation 2: Missing Page Request

![Simulation 2](screenshots/simulation2.png)

## Checkpoint 5: Container Logs and Metrics

I inspected the container logs using `docker logs clientwebsite`.

The logs showed Nginx startup messages, successful requests, and requests that returned HTTP 404.

### Docker Logs

![Docker Logs](screenshots/docker-logs.png)

I also used `docker stats clientwebsite` to monitor CPU usage, memory usage, network I/O, block I/O, and the number of processes.

### Container Metrics

![Container Metrics](screenshots/container-metrics.png)

## Skills Learned

- Linux system resource monitoring
- Docker container deployment
- HTTP request testing
- Nginx log analysis
- Container performance monitoring
- Technical documentation using Markdown

## Conclusion

This laboratory helped me understand how to monitor system resources, deploy a web server using Docker, test HTTP responses, and inspect container logs. I also learned how container metrics can help administrators understand resource usage and troubleshoot applications.
