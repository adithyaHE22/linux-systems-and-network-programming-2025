# Linux Systems & Network Programming – Full Project Documentation

This repository contains a complete, step-by-step implementation of Linux system administration and network services inside a virtual machine environment.  
The project includes Linux basics, server configurations, automation, security, and debugging using GDB.

---

## 📘 Project Overview

The objective of this project is to:

- Build a functional Linux environment using virtualization  
- Configure essential network services (DHCP, DNS, NTP)  
- Automate tasks using shell scripts and cron jobs  
- Set up secure remote access using SSH  
- Implement firewall rules with iptables  
- Deploy Apache and Postfix servers  
- Analyze executables using GDB and perform file decryption  

This README provides a clear, simple explanation of each step.

---

# 🖥️ 1. Linux Environment Setup

### ✔ Virtual Machine Setup
- Installed **VirtualBox**
- Downloaded **Ubuntu ISO**
- Created a VM with:
  - 2GB RAM  
  - 20GB storage  
  - Ubuntu 64-bit  

### ✔ Linux OS Installation
The OS was installed using the ISO image. User account, hostname, and system preferences were configured.

---

# 📂 2. Linux Command Line Basics

### Navigation Commands
- `pwd` → Show current directory  
- `cd` → Change directory  
- `ls` → List files  
- `ls -la` → List detailed files (including hidden)

### File Management
- `mkdir`, `rmdir`  
- `touch` (create file)  
- `cp` (copy)  
- `mv` (move/rename)  
- `cat` (read file)

### System Information
- `uname -a`  
- `df -h`  
- `free -h`  

---

# 🌐 3. Network Services Configuration

## ✔ DHCP Server (isc-dhcp-server)
- Installed DHCP server  
- Selected correct network interface  
- Configured IP range  
- Assigned gateway, DNS, domain name  
- Used Host-Only networking  
- Verified DHCP lease on client machine

## ✔ DNS Server (BIND9)
- Installed BIND9  
- Added Google DNS as forwarders  
- Configured local DNS zone  
- Linked zone files  
- Restarted BIND9 and tested domain resolution  
- Updated DHCP server to use the new DNS

## ✔ NTP Server
- Installed NTP service  
- Found correct config file (`/etc/ntpsec/ntp.conf`)  
- Added primary and fallback time servers  
- Restarted service and verified time synchronization  

---

# 🔐 4. Security & Other Server Configurations

## ✔ Shell Script Automation
- Created a script to:
  - Clean logs  
  - Archive logs  
- Automated using a Cron job (runs weekly)

## ✔ SSH Server
- Installed OpenSSH  
- Enabled and verified SSH service  
- Connected from a client machine

## ✔ iptables Firewall Rules
- Cleared existing firewall rules  
- Blocked social media websites  
- Allowed HTTPS  
- Blocked HTTP  
- Verified rule configurations

## ✔ Apache Web Server
- Installed Apache  
- Created HTML file  
- Set permissions  
- Accessed the web server from client machine  

## ✔ Postfix Email Server
- Installed Postfix  
- Selected “Internet Site” mode  
- Configured hostname  
- Sent and verified test email locally  

---

# 🐞 5. GDB Debugging & File Analysis

### Execution Analysis
- Checked system architecture  
- Selected correct executable  
- Program behavior:
  - Reads system UUID  
  - Encrypts using XOR  
  - Writes encrypted output to file  

### Debugging Steps (GDB)
- Loaded executable in GDB  
- Identified functions (`main`, `xor_encrypt_decrypt`)  
- Set breakpoints  
- Viewed assembly using `layout asm`  
- Captured function arguments  
- Traced encryption logic  

### File System Analysis
- Verified file type (`file`)  
- Checked content and permissions  
- Used `hexdump`  
- Wrote a C program to decrypt XOR output  
- Confirmed decrypted value matches system UUID  

---

# 📖 Conclusion

This project demonstrates strong understanding and practical skills in Linux systems and network administration.  
The work includes virtualization, server configuration, automation, security, web services, email services, debugging, and encryption analysis.

It provides a complete study reference for students learning Linux, networking, and system security.

---

# 📄 How to Use This Repository

1. Follow each section in order  
2. Use provided commands for replication  
3. Analyze logs, outputs, and scripts  
4. Refer to screenshots for guidance  

---


