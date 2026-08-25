# Infrastructure Report

## Operating System

```text
PRETTY_NAME="Ubuntu 24.04.4 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04.4 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo
```

## Kernel Version

```text
6.8.0-138-generic
```

## CPU Model

```text
Model name: Intel Xeon E312xx (Sandy Bridge, IBRS update)
```

## Number of CPU Cores

```text
1
```

## Total RAM

```text
               total        used        free      shared  buff/cache   available
Mem:           1.9Gi       418Mi       832Mi       1.1Mi       821Mi       1.5Gi
Swap:          1.0Gi          0B       1.0Gi
```

## Disk Capacity

```text
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           191M  996K  190M   1% /run
/dev/vda1        19G  5.4G   13G  30% /
tmpfs           952M   84K  952M   1% /dev/shm
tmpfs           5.0M     0     5.0M   0% /run/lock
/dev/vda16      881M  117M  703M  15% /boot
/dev/vda15      105M  6.2M   99M   6% /boot/efi
```

## Mounted File Systems

```text
TARGET                 SOURCE   FSTYPE   OPTIONS
/                      /dev/vda1
                                ext4     rw,relatime,discard,errors=remount-ro,commit=30
|-/sys                 sysfs    sysfs    rw,nosuid,nodev,noexec,relatime
| |-/sys/kernel/security
| |                    securityfs
| |                             security rw,nosuid,nodev,noexec,relatime
| |-/sys/fs/cgroup     cgroup2  cgroup2  rw,nosuid,nodev,noexec,relatime,nsdelegate,memory_
| |-/sys/fs/pstore     pstore   pstore   rw,nosuid,nodev,noexec,relatime
| |-/sys/fs/bpf        bpf      bpf      rw,nosuid,nodev,noexec,relatime,mode=700
| |-/sys/kernel/debug  debugfs  debugfs  rw,nosuid,nodev,noexec,relatime
| |-/sys/kernel/tracing
| |                    tracefs  tracefs  rw,nosuid,nodev,noexec,relatime
| |-/sys/kernel/config configfs configfs rw,nosuid,nodev,noexec,relatime
| `-/sys/fs/fuse/connections
|                      fusectl  fusectl  rw,nosuid,nodev,noexec,relatime
|-/proc                proc     proc     rw,nosuid,nodev,noexec,relatime
| `-/proc/sys/fs/binfmt_misc
|                      systemd-1
|                               autofs   rw,relatime,fd=32,pgrp=1,timeout=0,minproto=5,maxp
|   `-/proc/sys/fs/binfmt_misc
|                      binfmt_misc
|                               binfmt_m rw,nosuid,nodev,noexec,relatime
|-/dev                 udev     devtmpfs rw,nosuid,relatime,size=954836k,nr_inodes=238709,m
| |-/dev/pts           devpts   devpts   rw,nosuid,noexec,relatime,gid=5,mode=620,ptmxmode=
| |-/dev/shm           tmpfs    tmpfs    rw,nosuid,nodev,inode64
| |-/dev/hugepages     hugetlbfs
| |                             hugetlbf rw,nosuid,nodev,relatime,pagesize=2M
| `-/dev/mqueue        mqueue   mqueue   rw,nosuid,nodev,noexec,relatime
|-/run                 tmpfs    tmpfs    rw,nosuid,nodev,noexec,relatime,size=194892k,mode=
| `-/run/lock          tmpfs    tmpfs    rw,nosuid,nodev,noexec,relatime,size=5120k,inode64
`-/boot                /dev/vda16
                         ext4     rw,relatime
  `-/boot/efi          /dev/vda15
                         vfat     rw,relatime,fmask=0077,dmask=0077,codepage=437,ioc

## Hostname

```text
ubuntu
```

## IP Address

```text
172.30.1.2
172.17.0.1
```
