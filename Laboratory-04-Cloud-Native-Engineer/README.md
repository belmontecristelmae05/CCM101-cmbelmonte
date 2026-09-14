
# Laboratory 04 - Cloud-Native Engineer
---

## Mission Overview

This laboratory activity focused on learning how Docker containers are used in cloud-native environments. Using the KillerCoda Docker environment, I checked the Docker installation and environment, downloaded the Nginx image, ran an Nginx container, tested the web server, and managed the container lifecycle. The activity helped me understand how containers can provide a faster and more lightweight way of running applications.

---


## Objectives

- Explore how Docker works in a cloud-native environment.
- Practice using Docker through the KillerCoda terminal.
- Deploy and access an Nginx web server using a container.
- Learn how port mapping connects the host to the container.
- Practice stopping and removing a Docker container.
- Improve technical documentation and GitHub organization.

---

## Docker Commands Executed

### Checkpoint 3 - Docker Playground

```bash
docker --version
docker info
```

### Checkpoint 4 - Deploy Nginx

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
```


---

## Skills Learned

Through this laboratory activity, I learned how to use basic Docker commands to create, run, check, stop, and remove containers. I also learned the difference between virtual machines and containers and understood why containers are useful in cloud-native environments. The activity helped me become more familiar with the Linux terminal and Docker container management.

---

## Challenges Encountered

One challenge I encountered was understanding and using the different Docker commands correctly. I also needed to understand how the port mapping 8080:80 allowed me to access the Nginx web server through the host. Another challenge was managing the container from running it to stopping and removing it. Following the commands step by step helped me understand how Docker containers are deployed and managed.

```
