# Container Observability Report

## Overview

This report documents the deployment, traffic simulation, application logging, and resource monitoring of the Nginx web server using Docker.

## 1. Deploy the Nginx Container

### Command Executed

    docker run -d --name clientwebsite -p 8080:80 nginx

### Explanation

This command deploys an Nginx web server in the background. The container is named clientwebsite, and port 8080 on the host is mapped to port 80 inside the container.

### Verify the Container

    docker ps

This command displays the running containers and their status.

### Screenshot

- screenshots/install-nginx.png

## 2. Generate Web Traffic

### Successful HTTP Requests

Commands executed:

    curl http://localhost:8080
    curl http://localhost:8080
    curl http://localhost:8080

These commands simulate three visits to the website. The requests should return the default Nginx welcome page.

### Generate a Failed Request

Command executed:

    curl http://localhost:8080/hidden-admin-page

This command requests a nonexistent page. Nginx should return a 404 Not Found response.

### Check the HTTP Status Code

    curl -o /dev/null -s -w "HTTP Status: %{http_code}\n" http://localhost:8080/hidden-admin-page

Expected result:

    HTTP Status: 404

### Screenshots

- screenshots/simulation1.png
- screenshots/simulation2.png

## 3. Application Logging

### Command Executed

    docker logs clientwebsite

### Explanation

The docker logs command displays the output produced by the container. Nginx access logs help identify incoming HTTP requests and their response status codes.

### HTTP 404 Error Log

Paste the actual log line containing the 404 status code from your terminal below.

    [Paste your actual HTTP 404 log line here]

### Why Application Logs Are Important

Application logs help identify errors, failed requests, and unusual application behavior. They allow engineers to investigate problems and determine what happened instead of guessing about the cause.

### Screenshot

- screenshots/docker-logs.png

## 4. Real-Time Container Metrics

### Command Executed

    docker stats clientwebsite

### Explanation

The docker stats command displays real-time information about a running container's resource consumption. It helps engineers monitor CPU usage, memory consumption, and network activity.

### Recorded Metrics

Record the actual values displayed in your terminal.

- **Container Name:** clientwebsite
- **CPU Usage:** [Enter the actual CPU percentage]
- **Memory Usage:** [Enter the actual memory usage]
- **Memory Limit:** [Enter the displayed memory limit]
- **Network I/O:** [Enter the displayed network input/output values]

### Screenshot

- screenshots/container-metrics.png

## 5. Observability Findings

The Nginx container was used to simulate normal website visits and a request to a nonexistent page. Application logs provided evidence of the requests and their HTTP response codes, while Docker metrics showed the container's resource consumption.

The recorded values represent the container's condition at the time of monitoring. Additional testing with more concurrent requests would be needed to determine how the application behaves under a large traffic surge.

## Conclusion

This activity demonstrated how application logs and performance metrics support cloud operations. Logs help engineers investigate application events and errors, while metrics provide numerical information about resource usage and system performance.
