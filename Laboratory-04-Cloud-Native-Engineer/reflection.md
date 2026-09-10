# Mission 4 Reflection

This laboratory activity helped me understand the difference between Virtual Machines and containers and how Docker makes application deployment faster and easier. When using a Virtual Machine, installing an operating system requires more time because the VM needs to boot and run a complete operating system. In comparison, a Docker container can start in seconds because containers share the host operating system kernel. This makes containers more lightweight and efficient for applications such as web servers.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80, while port 8080 provides a way for the host machine to access that service. Without port mapping, the Nginx service would not be directly accessible through the host's port 8080. Using `curl http://localhost:8080` allowed me to test the connection and confirm that the Nginx server was working correctly.

When `docker rm` is used, the specified container is removed from the Docker environment. Data stored only inside the container that was not saved using persistent storage or volumes can be lost. This showed me why persistent data should be stored separately when an application needs to keep information after a container is removed.

Containerization also changes how developers and IT operations teams work together. Developers can package applications with their required dependencies, while operations teams can deploy the same containerized application in different environments. This supports DevOps by making development, testing, and deployment more consistent.

My GitHub portfolio is also evolving as I add more laboratory activities and technical documentation. Each laboratory gives me an opportunity to organize my work, record commands and results, and show the skills I have developed in cloud computing.
