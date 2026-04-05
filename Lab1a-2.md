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
