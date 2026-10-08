# Mission Reflection

This laboratory activity helped me understand the importance of monitoring a server and its containers. I learned that deploying an application is not enough because we also need to check its performance, identify errors, and make sure that it can run properly.

Checking the host server's resources is important even when containers are running perfectly. Containers depend on the host's CPU, RAM, and disk storage. If the server runs out of memory or disk space, the containers may become slow or stop working. Monitoring these resources helps us identify possible problems before they affect users.

The docker logs command is useful when a user reports that they cannot log into a web application. It allows an engineer to examine the application's logs and look for error messages, failed requests, or other events related to the problem. These details can help narrow down the possible cause and guide the next troubleshooting steps.

I also learned the difference between logs and metrics. Logs contain records of application events, requests, and errors. Metrics provide numerical measurements such as CPU usage, memory consumption, and network activity. Both are important because logs help explain what happened, while metrics help show how the system is performing.

Large enterprise companies can monitor thousands of containers using centralized monitoring tools such as Prometheus and Grafana. Prometheus collects and stores metrics, while Grafana presents monitoring data through dashboards and visualizations. These tools help engineers observe system performance and identify problems across many services.

My ability to troubleshoot Linux environments improved because I practiced using commands such as free -h, df -h /, top, docker logs, and docker stats. I became more familiar with checking system resources, examining application output, and monitoring containers. I also learned that troubleshooting should be based on actual evidence rather than assumptions.

Overall, this laboratory helped me understand that monitoring is an important part of cloud computing. It taught me to check system health, analyze application logs, and use performance metrics to help maintain reliable applications.
