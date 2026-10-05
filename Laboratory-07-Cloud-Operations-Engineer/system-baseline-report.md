# System Baseline Report

## Host System Baseline

### Total RAM

The server has a total of **1.9 GiB of RAM**.

### Total Root Storage

The root (/) file system has a total storage capacity of **19 GB**.

### Why Disk Space Is Important

Checking disk space before a massive traffic surge is critical because insufficient storage can prevent the server and applications from writing logs, temporary files, and other required data, which may cause service failures.

## Monitoring Command Used

```bash
free -h
df -h /
top
