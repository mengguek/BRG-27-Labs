# 🖥️ Ubuntu Virtual Machine Setup on macOS (Apple Silicon)

## 📌 Overview
This section documents the setup of an Ubuntu Linux environment on macOS using virtualization.  
The ARM64 version of Ubuntu is used for compatibility with Apple Silicon systems.

---

## ⚙️ Requirements
- macOS (Apple Silicon - M3 Pro)
- Oracle VM VirtualBox
- Ubuntu Desktop ISO (ARM64 version)

---

## 🚀 Installation Steps

### 1. Install VirtualBox
Download and install from:  
https://www.virtualbox.org/

---

### 2. Download Ubuntu ISO
Download Ubuntu Desktop (ARM64):  
https://ubuntu.com/download/desktop

---

### 3. Create Virtual Machine
- Open VirtualBox  
- Click **New**  
- Name: Ubuntu  
- Type: Linux  
- Version: Ubuntu (64-bit)  

---

### 4. Allocate Resources
- RAM: Minimum 2 GB  
- CPU: 1 core  
- Storage: 20 GB (dynamically allocated)  

---

### 5. Attach ISO File
- Go to **Settings → Storage**  
- Add the downloaded Ubuntu ISO  

---

### 6. Start Installation
- Start the VM  
- Follow Ubuntu installation prompts  
- Select default options  

---

## 📝 Notes
- ARM64 version is required for Apple Silicon  
- Ensure virtualization is enabled  
- Always download from official sources  

---

## ✅ Result
A functional Ubuntu environment was successfully installed on macOS, enabling Linux-based lab work and experimentation.
