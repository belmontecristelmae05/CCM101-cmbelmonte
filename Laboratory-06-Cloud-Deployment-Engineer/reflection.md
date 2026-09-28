# Mission Reflection

This laboratory helped me understand how Docker Compose can make cloud deployment easier and more organized. Instead of manually creating and configuring each container separately, I was able to define the required services in one `docker-compose.yml` file. This makes the deployment process more consistent because the same configuration can be used again when the application needs to be deployed.

I also learned that YAML files are sensitive to indentation. Using incorrect indentation or a Tab instead of spaces can cause the Compose file to become invalid or prevent Docker Compose from correctly understanding the configuration. Because of this, proper formatting is important when creating Infrastructure as Code files.

Environment variables such as `MYSQL_PASSWORD` were used to provide configuration information to the containers. They allowed the Nextcloud application and MariaDB database to use the required database credentials and connection information. The `MYSQL_HOST=database` setting also showed me how the Nextcloud container can identify the database service using its Docker Compose service name.

Deploying Nextcloud was a useful experience because I was able to see how several containers can work together as one application. The process showed me that a cloud storage system does not have to be deployed manually one component at a time when a configuration file can define the infrastructure.

Since Mission 1, my understanding of Cloud Computing has developed from simply learning about cloud concepts to actually working with containers and cloud deployment tools. I now understand more clearly how Docker, containers, networking, configuration files, and Infrastructure as Code can work together to deploy an application.
