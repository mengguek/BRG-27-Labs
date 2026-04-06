# Linux Services


---

## Nginx Web Server
### installing and configuring the Nginx webserver

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo apt update

```

<img width="750" height="760" alt="Screenshot 2026-04-06 at 22 05 03" src="https://github.com/user-attachments/assets/0c1f8345-1369-4e71-b0f7-a3e749133bc7" />

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo apt update


```
<img width="620" height="305" alt="Screenshot 2026-04-06 at 22 07 37" src="https://github.com/user-attachments/assets/f03d249c-572d-493c-8a73-4dd2756ea259" />

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo apt install nmap
```
<img width="474" height="311" alt="Screenshot 2026-04-06 at 22 09 32" src="https://github.com/user-attachments/assets/395edab9-0528-48f3-b3c0-442e5eb580c4" />

```bash
vboxuser@Ubuntu-Lab1a:-$ ssudo apt install openssh-server
```

<img width="516" height="326" alt="Screenshot 2026-04-06 at 22 10 58" src="https://github.com/user-attachments/assets/a9b583e2-85cd-4143-85a9-68071d057643" />

### Edit the Nginx web page
```bash
vboxuser@Ubuntu-Lab1a:-$ nano /var/www/html/index.nginx-debian.html
```
couldn't edit and faced this error as per screenshot
<img width="330" height="51" alt="Screenshot 2026-04-06 at 22 19 33" src="https://github.com/user-attachments/assets/24cd3aa6-b60c-4e1e-a47a-dfb8919a7bf4" />

```bash
vboxuser@Ubuntu-Lab1a:-$ gedit /var/www/html/index.nginx-debian.html
```
although the interface is different it pop a text file and could edit.

<img width="459" height="350" alt="Screenshot 2026-04-06 at 22 21 23" src="https://github.com/user-attachments/assets/a2aca062-2b9e-45a9-987c-f8faa821e56b" />


```bash
vboxuser@Ubuntu-Lab1a:-$ nano /var/www/html/index.html
```

<img width="642" height="308" alt="Screenshot 2026-04-06 at 22 24 37" src="https://github.com/user-attachments/assets/a3057a94-ec6d-4fec-8277-a0c3dc37065f" />

### UFW Fire wall of ubuntu

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo ufw status verbose
```

#### turning on of firewall

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo ufw enable
```

#### checking of firewall config ?

```bash
vboxuser@Ubuntu-Lab1a:-$ sudo ufw status verbose
```

<img width="270" height="87" alt="Screenshot 2026-04-06 at 22 39 37" src="https://github.com/user-attachments/assets/a6bd7d06-9cdb-4792-9a92-d47b97212b79" />

### Dealing with compressed archives

<img width="631" height="217" alt="Screenshot 2026-04-06 at 22 49 09" src="https://github.com/user-attachments/assets/13c70bae-f80e-46fb-a26c-64e1e9042a49" />

<img width="311" height="270" alt="Screenshot 2026-04-06 at 22 49 22" src="https://github.com/user-attachments/assets/eeda5485-f346-4d2c-a868-017c90496e8d" />










