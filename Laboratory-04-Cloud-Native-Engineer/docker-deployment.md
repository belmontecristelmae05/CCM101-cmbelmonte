# Docker Deployment

## Checkpoint 3 - Enter the Docker Playground

### 1. Check Docker Version

```bash
docker --version
```

This command checks if Docker is installed and displays the installed Docker version.

### 2. Check Docker Information

```bash
docker info
```

This command displays detailed information about the Docker environment.

---

## Checkpoint 4 - Deploy Your First Container

### 1. Pull Nginx Image

```bash
docker pull nginx
```

This command downloads the Nginx image from Docker Hub.

### 2. Run Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command runs the Nginx container in the background and maps port 8080 to port 80.

### 3. Check Running Container

```bash
docker ps
```

This command shows the currently running Nginx container.

### 4. Test Nginx Web Server

```bash
curl http://localhost:8080
```

This command checks if the Nginx web server is running successfully.

---

## The Container Lifecycle

A Cloud-Native Engineer must know how to manage running containers. The following commands were used to list, stop, verify, and remove the Nginx container.

### 1. List Running Containers

```bash
docker ps
```

This command lists all currently running Docker containers and shows that the Nginx container is running.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 3. Verify It Is Stopped

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### To view the stopped container

```bash
docker ps -a
```

This command displays all containers, including stopped containers, and shows the Nginx container with an `Exited` status.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command completely removes the stopped Nginx container.

### Verify Container Removal

```bash
docker ps -a
```

This command verifies that the Nginx container has been completely removed and no longer appears in the container list.

## Screenshot

### Container Lifecycle

![Container Lifecycle](screenshots/container-lifecycle.png)
