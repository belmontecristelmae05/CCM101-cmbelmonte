# Docker Deployment

## Docker Environment Verification

### Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version and confirms that Docker is available in the environment.

### Check Docker Environment

```bash
docker info
```

This command displays detailed information about the Docker environment, including the Docker server, containers, images, storage, and operating system.

---

## Nginx Deployment

### Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub.

### Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and runs an Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### Check the Running Container

```bash
docker ps
```

This command lists the containers that are currently running.

### Test the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx web server and verifies that it is responding successfully.

---

## Container Lifecycle

### List Running Containers

```bash
docker ps
```

This command displays all currently running containers.

### Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### Verify the Container Is Stopped

```bash
docker ps
```

This command confirms that the Nginx container is no longer running.

### View All Containers

```bash
docker ps -a
```

This command displays both running and stopped containers so the stopped Nginx container can be verified.

### Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container.

### Verify Container Removal

```bash
docker ps -a
```

This command verifies that the removed Nginx container no longer appears in the container list.
