
# Laboratory 08 - Cloud Security Engineer

## Mission Overview

The mission of this laboratory activity is to learn how to secure a server using basic cloud security practices. The activity includes deploying an Nginx web server using Docker, configuring the UFW firewall, and allowing the required network port. These tasks help protect the server from unauthorized access.

## Objectives

- Understand the Principle of Least Privilege (PoLP).
- Identify the attack surface of a virtual machine.
- Understand the importance of a Default Deny Policy.
- Deploy an Nginx web server using Docker.
- Configure and activate the UFW firewall.
- Allow the required port for the web application.
- Verify firewall rules and test the web server.
- Capture screenshots as evidence of completed tasks.

## Commands Executed

### Checkpoint 3 - Deploy the Web Server

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Checkpoint 4 - Configure the Firewall

```bash
sudo ufw version
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
```

### Checkpoint 5 - Allow the Required Port

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl http://localhost:8080
docker ps
```

## Skills Learned

In this laboratory activity, I learned how to deploy an Nginx web server using Docker and check if the container is running properly. I learned how to configure and activate the UFW firewall to manage incoming and outgoing network traffic. I also learned how to allow a specific port for a web application and verify the firewall rules using terminal commands. Additionally, I understood the importance of the Principle of Least Privilege, reducing the attack surface, and applying a Default Deny Policy to improve server security. Lastly, I practiced documenting commands and organizing screenshots as evidence of the completed laboratory tasks.

