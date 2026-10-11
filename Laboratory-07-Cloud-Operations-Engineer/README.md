
# Laboratory 7 - The Cloud Operations Engineer

## Mission Overview

The mission of this laboratory activity is to monitor server resources, deploy an Nginx container using Docker, simulate HTTP requests, and inspect container logs and resource usage.

## Objectives

- Check the server's available RAM and root filesystem storage.
- Deploy and run an Nginx container using Docker.
- Test successful and unsuccessful HTTP requests.
- Inspect Docker logs to identify requests and errors.
- Monitor container CPU and memory usage.

## Monitoring Commands Executed

### 1. Check Available RAM

```bash
free -h
```

### 2. Check Root Filesystem Storage

```bash
df -h /
```

### 3. Monitor System Resources

```bash
top
```

### 4. Deploy the Nginx Container

```bash
docker run -d --name clientwebsite -p 8080:80 nginx
```

### 5. Check Container Status

```bash
docker ps -a
docker ps
```

### 6. Simulate HTTP Requests

```bash
curl http://localhost:8080
curl -I http://localhost:8080
curl http://localhost:8080/hidden-admin-page
curl -o /dev/null -s -w "HTTP Status: %{http_code}\n" http://localhost:8080/hidden-admin-page
```

The Nginx homepage returned HTTP status code 200, while the request to `/hidden-admin-page` returned HTTP status code 404.

### 7. Check Container Logs

```bash
docker logs clientwebsite
```

### 8. Monitor Container Metrics

```bash
docker stats clientwebsite
```

## Skills Learned

In this laboratory activity, I learned how to check the server's available RAM and disk space using Linux commands. I also learned how to deploy and run an Nginx container using Docker. I learned how to test HTTP requests and understand the difference between status codes 200 and 404. I also learned how to check Docker logs to identify requests and errors. Lastly, I learned how to monitor container CPU and memory usage using the `docker stats` command.


