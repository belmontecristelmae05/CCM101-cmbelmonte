# System Baseline Report

## Overview

This report documents the initial health check of the Linux host server using the KillerCoda Playground. The purpose is to identify the available system resources before deploying and monitoring the Nginx web server.

## 1. Memory Usage

### Command Executed

    free -h

### Results

- **Total RAM:** [Enter the total RAM displayed in your terminal]
- **Used RAM:** [Enter the used RAM displayed in your terminal]
- **Available RAM:** [Enter the available RAM displayed in your terminal]

### Explanation

Checking memory usage helps determine whether the server has enough available RAM to run containers and handle application requests without experiencing memory shortages.

## 2. Disk Storage

### Command Executed

    df -h /

### Results

- **Root File System:** /
- **Total Storage Capacity:** [Enter the Size value]
- **Used Storage:** [Enter the Used value]
- **Available Storage:** [Enter the Avail value]
- **Disk Usage:** [Enter the Use% value]

### Explanation

Checking disk space before a massive traffic surge is important because insufficient storage can prevent applications from writing logs, storing temporary files, and operating correctly.

## 3. CPU and Running Processes

### Command Executed

    top

### Observations

- **CPU Usage:** [Enter your observation]
- **System Load:** [Enter your observation]
- **Running Processes:** [Enter your observation]

### Explanation

The top command displays active processes, CPU utilization, memory usage, and system load in real time. Monitoring these values helps identify processes that may consume excessive system resources.

## 4. Screenshots

The following screenshots provide evidence of the host system baseline check:

- screenshots/memory-check.png
- screenshots/disk-check.png

## Conclusion

The host system baseline check provided information about the server's available memory, disk capacity, and CPU activity. These measurements serve as a reference for understanding system health while the Nginx container is running.
