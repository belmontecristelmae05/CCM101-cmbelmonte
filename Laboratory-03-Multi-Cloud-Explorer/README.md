
## Linux Server Investigation Using KillerCoda

The Linux server provided in the KillerCoda Playground was investigated using basic Linux commands. The investigation focused on identifying the operating system, CPU information, memory, and disk space of the server.

---

## 1. Operating System

Use the following command to identify the operating system:

```bash
uname -a
````

**Result:**
- OS: Ubuntu 24.04
- Kernel: Linux 6.8.0-13-generic
- Architecture: x86_64
- System: GNU/Linux

### Terminal Evidence 1 – Operating System
![Operating System](https://github.com/user-attachments/assets/ceccc8e9-4038-4c5d-8de1-1534478a4294)

---

## 2. CPU Information

Use the following command to identify the CPU information:

```bash
lscpu
```
**Result:**
- Architecture: x86_64
- CPU(s): 1
- Model: Intel Xeon E312xx (Sandy Bridge, IBRS update)
- CPU Frequency: 2.00 GHz

### Terminal Evidence 2 – CPU Information
![CPU](https://github.com/user-attachments/assets/752b3413-b1a0-4266-8c19-fa718b79bf07)

---

## 3. Memory

Use the following command to identify the available memory:

```bash
free -h
```

**Result:**
- Total Memory: 1.9 GiB
- Available Memory: 1.5 GiB
- Swap: 1.0 GiB

### Terminal Evidence 3 – Memory
![Memory](https://github.com/user-attachments/assets/e13fc0f9-e82f-44fc-86f0-d05d93489dc6)

---

## 4. Disk Space

Use the following command to identify the disk space:

```bash
df -h
```

**Result:** 
- Total Disk Space: 19 GB
- Available Disk Space: 13 GB
- Disk Usage: 30%

### Terminal Evidence 4 – Disk Space
![Disk Space](https://github.com/user-attachments/assets/c5497ca3-bebe-4897-b675-6c2ab90e847a)

---

## Linux System Information Summary

| Information      | Linux Command         | Result                                                                                  |
| ---------------- | --------------------- | ------------------------------------------ |
| Operating System | `uname -a`            |  Ubuntu 24.04, Linux 6.8.0-13-generic, x86_64, GNU/Linux |
| CPU Information  | `lscpu`               | x86_64, 1 CPU, Intel Xeon E312xx, 2.00 GHz |
| Memory           | `free -h`             | 1.9 GiB total, 1.5 GiB available             |
| Disk Space       | `df -h`               | 19 GB total, 13 GB available disk space                             |

---

## Cloud Migration

The Linux server identified in the KillerCoda Playground can be migrated to a cloud platform using a virtual machine service.

| Cloud Provider | Service |
|---|---|
| AWS | Amazon EC2 |
| Microsoft Azure | Azure Virtual Machines |
| Google Cloud Platform (GCP) | Compute Engine |

These services can host the Linux server in the cloud.



---
