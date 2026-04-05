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
### Super User

```bash
vboxuser@Ubuntu-Lab1a:-$ whoami
vboxuser
```
#### not allowed to access root directly
```bash
vboxuser@Ubuntu-Lab1a:-$ adduser newuser
adduser: Permission denied
```
#### sudo allows temporary root access
```bash
vboxuser@Ubuntu-Lab1a:-$ sudo whoami
root
```
#### managed to create the newuser account on linux
```bash
vboxuser@Ubuntu-Lab1a:-$ sudo adduser newuser
(creates new user successfully)
```
### Network Configuration
```bash
vboxuser@Ubuntu-Lab1a:-$ ip a

```
 <img width="647" height="322" alt="Screenshot 2026-04-05 at 21 18 41" src="https://github.com/user-attachments/assets/ad6fe27a-1891-4a7d-bd4b-3f2c4b88bd35" />

```bash
vboxuser@Ubuntu-Lab1a:-$  ping 134.115.148.1

```
<img width="655" height="434" alt="Screenshot 2026-04-05 at 21 20 49" src="https://github.com/user-attachments/assets/8260c6f8-4f74-4934-b361-abc285758432" />

#### The address works at home because it is part of a local network environment, and access depends on being connected to the same network as the service.

```bash
vboxuser@Ubuntu-Lab1a:-$ ping 8.8.8.8

```


<img width="662" height="488" alt="Screenshot 2026-04-05 at 21 23 17" src="https://github.com/user-attachments/assets/590a6f6a-fceb-4a10-a49f-1dfad521061c" />
### Hosts

```bash
vboxuser@Ubuntu-Lab1a:-$  less /etc/hosts

```

<img width="657" height="492" alt="Screenshot 2026-04-05 at 21 38 45" src="https://github.com/user-attachments/assets/c71206f9-d88c-4e39-87a6-e0532861ff79" />

```bash
vboxuser@Ubuntu-Lab1a:-$   ping localhost

```

<img width="673" height="343" alt="Screenshot 2026-04-05 at 21 39 55" src="https://github.com/user-attachments/assets/1b38a4c7-ae14-4618-a396-c96c55a15863" />

 ```bash
vboxuser@Ubuntu-Lab1a:-$ sudo nano /etc/hosts
```
<img width="654" height="506" alt="Screenshot 2026-04-05 at 21 46 38" src="https://github.com/user-attachments/assets/d4526407-107e-4e04-9b0a-a3986695e6e0" />

#### After adding  8.8.8.8 GoogleEpicDNS
<img width="642" height="481" alt="Screenshot 2026-04-05 at 21 55 43" src="https://github.com/user-attachments/assets/dc0cfa0b-0fa3-4ce0-b2f3-04650e466240" />


### DNS

 ```bash
vboxuser@Ubuntu-Lab1a:-$ nslookup google.com
```

<img width="660" height="579" alt="Screenshot 2026-04-05 at 22 02 35" src="https://github.com/user-attachments/assets/bd47ecfb-09bc-4683-a37f-aaf336682dbe" />
#### Installation of whois
 ```bash
vboxuser@Ubuntu-Lab1a:-$  sudo apt install whois
```
<img width="703" height="578" alt="Screenshot 2026-04-05 at 22 04 09" src="https://github.com/user-attachments/assets/7c0bfe8b-1107-48ac-9644-d3d1cc58e083" />

#### it contains an email address in the case that we have a complaint to make.
 ```bash
vboxuser@Ubuntu-Lab1a:-$ whois google.com
```

 <img width="652" height="487" alt="Screenshot 2026-04-05 at 22 07 58" src="https://github.com/user-attachments/assets/1a73f36f-1dc4-4d59-b83e-74822c172419" />

### Public and Private IP addresses

```bash
vboxuser@Ubuntu-Lab1a:-$ ip a
```
<img width="594" height="291" alt="Screenshot 2026-04-05 at 22 12 17" src="https://github.com/user-attachments/assets/3616fa51-7916-408c-b350-885c16c604af" />

### Hardware

 ```bash
vboxuser@Ubuntu-Lab1a:-$ lsusb
```
<img width="642" height="310" alt="Screenshot 2026-04-05 at 22 19 07" src="https://github.com/user-attachments/assets/3efea8e6-ea38-4eb3-b5c4-57aa5f1154f7" />
 
 ```bash
vboxuser@Ubuntu-Lab1a:-$ lspci
```
  <img width="642" height="312" alt="Screenshot 2026-04-05 at 22 20 01" src="https://github.com/user-attachments/assets/59ee9157-8809-47b3-b70b-5e471df1fac7" />

 ```bash
vboxuser@Ubuntu-Lab1a:-$ less /proc/cpuinfo
```
<img width="637" height="314" alt="Screenshot 2026-04-05 at 22 18 20" src="https://github.com/user-attachments/assets/3b433aa3-b6ff-4ed1-88fd-4315a1ef0966" />

   
Find "About this Computer", which is located under settings in the GUI. 
Is it more or less useful?- Less Useful
Which do you prefer?


