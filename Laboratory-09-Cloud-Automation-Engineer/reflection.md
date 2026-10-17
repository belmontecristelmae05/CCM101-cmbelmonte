# Mission Reflection

Automation is critical when managing hundreds of cloud servers because it makes repetitive tasks faster and easier to manage. Instead of configuring each server manually, administrators can use scripts to perform tasks such as creating backups, checking resources, and managing services. Automation also helps maintain consistency and reduces human errors when tasks are performed correctly.

However, automation also has potential dangers. A small mistake in a script can cause serious problems, especially when it runs on many servers. For example, if a script contains a destructive command or an incorrect file path and runs on 1,000 servers, it could delete important files or damage services across the entire environment. This is why scripts should be reviewed, tested on a small number of servers, and checked carefully before being deployed widely.

Writing a Bash script was different from creating a Docker Compose YAML file in Mission 6. Bash uses commands and programming logic to perform tasks step by step. In this mission, I used a Bash script to create a compressed backup of a directory and added a Cron schedule to automate its execution. Docker Compose YAML, on the other hand, uses a structured configuration format to define and manage containers, services, and their settings. Bash focuses on executing tasks, while Docker Compose focuses on describing how containerized applications should run.

From Laboratory 1 to Laboratory 9, my understanding of Cloud Computing developed from learning basic concepts and commands to understanding how cloud environments are deployed, managed, monitored, secured, and automated. Each laboratory helped me see how different cloud technologies and responsibilities work together to keep systems reliable and efficient.

The role I enjoyed the most was Cloud Automation Engineer because I learned how scripts can reduce repetitive manual work. Creating the backup script and scheduling it with Cron helped me understand how automation can make cloud operations more efficient. This mission also taught me that automation requires careful planning, testing, and monitoring to avoid problems.
