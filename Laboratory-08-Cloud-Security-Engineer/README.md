# Laboratory Activity 8: The Cloud Security Engineer

## Mission Overview

In this laboratory activity, I deployed an Nginx web server using Docker and configured the UFW firewall in a Linux environment. The activity focuses on securing a web application by controlling incoming network connections and allowing only the required ports.

## Objectives

- Deploy an Nginx web server using Docker.
- Check whether the web application is running.
- Configure the UFW firewall.
- Apply the Principle of Least Privilege (PoLP).
- Configure default firewall policies.
- Allow SSH and the required web application port.
- Document the security configuration and its importance.

## Commands Executed

### Check Docker

```bash
docker --version


Deploy the Nginx Container
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
```

### Check and Configure UFW
```bash
sudo ufw version
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
```

### Allow the Web Application Port
```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl http://localhost:8080
docker ps
```

### Skills Learned
- Deploying web applications with Docker
- Configuring a Linux firewall
- Managing network ports
- Applying basic security principles
- Checking container status and web connectivity
- Documenting technical work using Markdown
  
### Screenshots
The following screenshots should be saved in the screenshots/ folder.
- vulnerable-app-running.png
- firewall-activated.png
- firewall-port-allowed.png
  
### Conclusion
This activity helped me understand the importance of firewall configuration and network access control. I learned how to deploy an Nginx container, configure firewall rules, and check whether the application responds. Proper security configuration helps reduce unnecessary network exposure.
