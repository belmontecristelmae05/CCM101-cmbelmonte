
# Mission Reflection

In this laboratory activity, I learned that checking the host server's resources is important even when containers are running perfectly. Containers still depend on the host server's CPU, RAM, and disk space. If the server runs out of memory or storage, applications may become slow or stop working properly. Regular monitoring helps prevent problems and keeps applications running smoothly.

If a user cannot log in to a web application, I would use the `docker logs` command to check the container's logs. The logs may show error messages, failed requests, or other problems that can help me understand what happened. By examining these messages, I can identify possible causes of the login issue and decide what steps to take to fix it.

Monitoring logs and monitoring metrics have different purposes. Logs show recorded events, requests, and errors that happen inside an application. Metrics show numerical information about the container's performance, such as CPU usage, memory consumption, and network activity. Logs help explain what happened, while metrics help determine how well the system is performing.

Large enterprise companies may use monitoring tools such as Prometheus and Grafana to monitor thousands of containers at the same time. Prometheus collects and stores metrics from different systems, while Grafana displays the collected information through dashboards and graphs. These tools help engineers monitor performance, identify unusual activity, and detect possible problems more efficiently.

This activity also improved my ability to troubleshoot Linux environments. I became more familiar with commands such as `free -h`, `df -h /`, `docker logs`, and `docker stats`. I learned how to check system resources, examine application errors, and monitor container performance. These skills helped me understand how to investigate problems instead of simply guessing their causes. I can use what I learned in future activities involving Linux, Docker, and cloud computing.

