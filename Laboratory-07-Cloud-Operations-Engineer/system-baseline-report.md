# System Baseline Report

## 1. Host System Baseline

Before deploying the client's web server, a baseline health check was performed on the Linux host. The purpose of the baseline check was to determine the server's current memory and storage resources before running the containerized application.

The host system was checked using the `free -h`, `df -h /`, and `top` commands.

## 2. Memory Check

The `free -h` command was used to check the current memory resources of the server.

### Command Executed

```bash
free -h
```

### Memory Results

Based on the terminal output, the server has the following memory resources:

| Memory Information | Value |
|---|---:|
| Total RAM | 1.9Gi |
| Used RAM | 414Mi |
| Free RAM | 1.1Gi |
| Available RAM | 1.5Gi |
| Swap | 0B |

The server has a total of **1.9Gi of RAM**. At the time of the baseline check, **414Mi** was being used and **1.5Gi** was available.

## 3. Disk Storage Check

The `df -h /` command was used to check the storage capacity of the root (`/`) file system.

### Command Executed

```bash
df -h /
```

### Disk Results

Based on the terminal output:

| Storage Information | Value |
|---|---:|
| File System | /dev/vda1 |
| Total Storage | 19G |
| Used Storage | 5.4G |
| Available Storage | 13G |
| Usage | 30% |
| Mount Point | / |

The root (`/`) file system has a total storage capacity of **19G**. At the time of the baseline check, **5.4G** was used and **13G** was available, with the disk currently at **30% usage**.

## 4. CPU and Process Monitoring

The `top` command was used to view the active processes and observe the CPU activity of the host server.

### Command Executed

```bash
top
```

The command was allowed to run for approximately five seconds so that the changing CPU metrics and active processes could be observed. The `q` key was then used to exit the `top` interface.

## 5. Importance of Checking Disk Space

Checking disk space before a massive traffic surge is critical because insufficient storage can prevent the server from properly storing application logs, temporary files, and other data required for reliable operation.

## 6. Baseline Summary

The baseline check provides an initial reference for the condition of the Linux host before deploying and monitoring the web application.

The server has **1.9Gi of total RAM** and **19G of total root storage**. The memory check showed **1.5Gi of available memory**, while the disk check showed **13G of available storage** and **30% disk usage** at the time of the assessment.

These baseline values can be used as a reference when examining the server and container performance during the succeeding checkpoints.
