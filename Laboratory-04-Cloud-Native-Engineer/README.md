# Laboratory 04 - The Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I explored the difference between traditional Virtual Machines and containers. I used the KillerCoda Docker environment to practice basic Docker commands and deployed an Nginx web server inside a container. I also learned how to manage the container lifecycle and document the procedures using Markdown.

## Objectives

- Differentiate between Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull and run a containerized Nginx application.
- Manage and terminate a Docker container.
- Document container operations using Markdown.
- Maintain an organized GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Check Docker Version

```bash
docker --version
```

### Check Docker Environment

```bash
docker info
```

### Pull Nginx Image

```bash
docker pull nginx
```

### Run Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

### List Running Containers

```bash
docker ps
```

### Test Nginx Web Server

```bash
curl http://localhost:8080
```

### Stop the Container

```bash
docker stop nginx-server
```

### View All Containers

```bash
docker ps -a
```

### Remove the Container

```bash
docker rm nginx-server
```

### Verify Container Removal

```bash
docker ps -a
```

## Skills Learned

- Understanding the difference between Virtual Machines and containers.
- Using Docker CLI commands.
- Pulling images from Docker Hub.
- Creating and running Docker containers.
- Mapping ports between the host and a container.
- Testing a containerized web server.
- Managing the container lifecycle.
- Creating technical documentation using Markdown.
- Organizing and maintaining a GitHub portfolio.

## Challenges Encountered

One challenge I encountered was understanding the difference between a Virtual Machine and a container. I also needed to become familiar with Docker commands and the purpose of port mapping. Running the Nginx container helped me understand how containers can make application deployment faster and easier. Another challenge was organizing the screenshots and Markdown files correctly in the GitHub repository.
