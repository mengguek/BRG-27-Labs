# Ubuntu Familiarisation Lab

---

## GUI Familiarisation

(Performed basic navigation using the Ubuntu graphical interface)

---

## CLI Familiarisation

### Process Listing

```bash
vboxuser@Ubuntu-Lab1a:-$ ps -e
PID   TTY   TIME     CMD
1     ?     00:00:02 systemd
1005  ?     00:00:00 dbus-daemon
1145  ?     00:00:01 NetworkManager
1372  ?     00:00:00 gdm3
2082  ?     00:01:34 gnome-shell
```
### System Monitor
```bash
vboxuser@Ubuntu-Lab1a:-$ top
top - load average: 0.20, 0.20, 0.18
Tasks: 195 total, 1 running, 190 sleeping
%Cpu(s): 20.0 us, 10.0 sy, 70.0 id
MiB Mem : 1627 total, 1154 used, 149 free
```
### Listing Files
#### ls for basic listing
```bash
vboxuser@Ubuntu-Lab1a:-$ ls
Desktop  Documents  Downloads  Pictures  session.txt
```
#### ls -la for detailed + hidden files
```bash
vboxuser@Ubuntu-Lab1a:-$ ls -la
(total output showing hidden files, permissions, and details)
```
### Creating and Editing Files
#### File created in /home/vboxuser
```bash
vboxuser@Ubuntu-Lab1a:-$ touch testfile
```
#### Faced issue for this as there is no GUI for it
```bash
vboxuser@Ubuntu-Lab1a:-$ gedit testfile
```
#### For nano it works in both local and remote terminal environments  
```bash
vboxuser@Ubuntu-Lab1a:-$ nano testfile
```
### Viewing File Contents

#### testfile content displayed fully (full output)
```bash
vboxuser@Ubuntu-Lab1a:-$ cat testfile

```
#### testfile content displayed with scrolling (scrollable)
```bash
vboxuser@Ubuntu-Lab1a:-$ less testfile

```
### Copying and Moving Files
#### Copying of files
```bash
vboxuser@Ubuntu-Lab1a:-$ cp testfile testfile2
```
#### Results
```bash
vboxuser@Ubuntu-Lab1a:-$ ls
Desktop Documents Downloads testfile testfile2
```
#### Moving(Renaming) of files
```bash
vboxuser@Ubuntu-Lab1a:-$ mv testfile2 testfile3
```
#### Results
```bash
vboxuser@Ubuntu-Lab1a:-$ ls
Desktop Documents Downloads testfile testfile3
```

### System Information
#### Displays detailed system information including the **kernel version, system architecture, and hostname**.
```bash
vboxuser@Ubuntu-Lab1a:-$ uname -a
Linux Ubuntu-Lab1a ... (kernel version and architecture)
```
#### Shows information about the Linux distribution, such as Ubuntu version and release details.
```bash
vboxuser@Ubuntu-Lab1a:-$ lsb_release -a
Distributor ID: Ubuntu
Description: Ubuntu ...
Release: ...
```
####  Provides system identity information including the hostname, operating system, and kernel, in a more structured format.
```bash
vboxuser@Ubuntu-Lab1a:-$ hostnamectl
Static hostname: Ubuntu-Lab1a
Operating System: Ubuntu
Kernel: Linux ...
```
### Sorting by Time (list files)
#### files sorted by most recent modification time
```bash
vboxuser@Ubuntu-Lab1a:-$ ls -alt

total 144
-rw-rw-r--  1 vboxuser vboxuser 61440 Apr  3 21:30 session.txt
drwxr-x--- 16 vboxuser vboxuser  4096 Apr  3 21:30 [0m[01;34m.[0m
-rw-rw-r--  1 vboxuser vboxuser     0 Apr  3 21:29 testfile3
drwx------ 17 vboxuser vboxuser  4096 Apr  3 21:26 [01;34m.config[0m
-rw-rw-r--  1 vboxuser vboxuser     0 Apr  3 21:25 testfile
-rw-------  1 vboxuser vboxuser    47 Apr  3 21:23 .bash_history
drwx------ 13 vboxuser vboxuser  4096 Apr  3 16:52 [01;34m.cache[0m
drwx------  2 vboxuser vboxuser  4096 Apr  3 16:52 [01;34m.gnupg[0m
drwx------  5 vboxuser vboxuser  4096 Mar 31 01:53 [01;34msnap[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mMusic[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mTemplates[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mDocuments[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mPublic[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mDownloads[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mVideos[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mPictures[0m
drwxr-xr-x  2 vboxuser vboxuser  4096 Mar 31 01:51 [01;34mDesktop[0m
drwx------  4 vboxuser vboxuser  4096 Mar 31 01:51 [01;34m.local[0m
drwx------  2 vboxuser vboxuser  4096 Mar 31 01:50 [01;34m.ssh[0m
drwxr-xr-x  3 root     root      4096 Mar 31 01:49 [01;34m..[0m
-rw-r--r--  1 vboxuser vboxuser   220 Sep  8  2025 .bash_logout
-rw-r--r--  1 vboxuser vboxuser   807 Sep  8  2025 .profile
-rw-r--r--  1 vboxuser vboxuser  3771 Sep  8  2025 .bashrc

```

















