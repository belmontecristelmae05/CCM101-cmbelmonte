
# Laboratory 04 - Cloud-Native Engineer
---

## Mission Overview

This laboratory activity focused on learning how Docker containers are used in cloud-native environments. Using the KillerCoda Docker environment, I checked the Docker installation and environment, downloaded the Nginx image, ran an Nginx container, tested the web server, and managed the container lifecycle. The activity helped me understand how containers can provide a faster and more lightweight way of running applications.

---

## Objectives

- Differentiate Virtual Machines from Containers.
- Access a Docker-enabled environment using KillerCoda.
- Verify that Docker is installed and running.
- Execute basic Docker CLI commands.
- Pull and run an Nginx container.
- Use port mapping to access a web server inside a container.
- Test the Nginx web server using curl.
- Stop and remove a Docker container.
- Document Docker commands using Markdown.
- Organize laboratory work in a GitHub portfolio.

---

## Docker Commands Executed

### Checkpoint 3 - Verify Docker

```bash
docker --version
````

This command checks the installed Docker version.

```bash
docker info
```

This command displays detailed information about the Docker environment and confirms that Docker is running properly.

### Checkpoint 4 - Deploy Nginx

```bash
docker pull nginx
```

This command downloads the Nginx image from Docker Hub.

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command runs the Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

```bash
docker ps
```

This command shows the running Nginx container and its port mapping.

```bash
curl http://localhost:8080
```

This command sends a request to the Nginx web server and displays the Nginx welcome page in the terminal.

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
```

This command lists the running Nginx container.

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

```bash
docker ps -a
```

This command displays all containers, including the stopped Nginx container.

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container completely.

```bash
docker ps -a
```

This command verifies that the Nginx container has been removed.

---

## Skills Learned

* Using basic Docker CLI commands
* Checking the Docker environment
* Pulling Docker images
* Running Docker containers
* Using port mapping
* Deploying an Nginx web server
* Testing a containerized web server
* Managing the container lifecycle
* Using the Linux terminal
* Creating technical documentation using Markdown
* Organizing files and screenshots in GitHub

---

## Challenges Encountered

One challenge I encountered was understanding and using the different Docker commands correctly. I also needed to understand how the port mapping `8080:80` allowed me to access the Nginx web server through the host. Another challenge was managing the container from running it to stopping and removing it. Following the commands step by step helped me understand how Docker containers are deployed and managed.

```
