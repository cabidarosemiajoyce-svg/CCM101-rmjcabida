# Mission 3 – Multi-Cloud Explorer

## Checkpoint 7 – Linux Investigation Using KillerCoda

A Linux environment was investigated using KillerCoda. The investigation focused on identifying the operating system, CPU information, memory, and disk space using basic Linux commands.

---

## 1. Operating System

The following command was used to identify the Linux operating system and its version:

```bash
cat /etc/os-release
```

The command displays information about the Linux distribution and version installed in the KillerCoda environment.

### Terminal Evidence 1 – Operating System

![KillerCoda Terminal 1 - Operating System](screenshots/killercoda-terminal-1.png)

---

## 2. CPU Information

The following command was used to check the CPU information of the Linux environment:

```bash
lscpu
```

The command displays information about the processor, including the CPU architecture, number of CPUs, and processor details.

### Terminal Evidence 2 – CPU Information

![KillerCoda Terminal 2 - CPU Information](screenshots/killercoda-terminal-2.png)

---

## 3. Memory

The following command was used to check the memory available in the Linux environment:

```bash
free -h
```

The command displays memory information in a human-readable format, including total, used, free, and available memory.

### Terminal Evidence 3 – Memory

![KillerCoda Terminal 3 - Memory](screenshots/killercoda-terminal-3.png)

---

## 4. Disk Space

The following command was used to check the available and used disk space:

```bash
df -h
```

The command displays the size, used space, available space, and usage percentage of the mounted file systems.

### Terminal Evidence 4 – Disk Space

![KillerCoda Terminal 4 - Disk Space](screenshots/killercoda-terminal-4.png)

---

## Linux System Information Summary

| System Information | Command Used | Result |
|---|---|---|
| Operating System | `cat /etc/os-release` | See Terminal Evidence 1 |
| CPU Information | `lscpu` | See Terminal Evidence 2 |
| Memory | `free -h` | See Terminal Evidence 3 |
| Disk Space | `df -h` | See Terminal Evidence 4 |

---

## Cloud Migration

If this Linux server were migrated to the cloud, it could be hosted using virtual machine services from AWS, Microsoft Azure, and Google Cloud Platform.

| Cloud Provider | Service That Could Host the Linux Server |
|---|---|
| AWS | Amazon EC2 |
| Microsoft Azure | Azure Virtual Machines |
| Google Cloud Platform (GCP) | Compute Engine |

These cloud services provide virtual computing environments that can be used to run Linux-based workloads.

## Conclusion

The KillerCoda investigation demonstrated how basic Linux commands can be used to examine a computer environment. The operating system, CPU, memory, and disk information were identified using standard Linux commands. The investigation also showed how a Linux server could be migrated to a cloud environment using virtual machine services from AWS, Microsoft Azure, or Google Cloud Platform.
