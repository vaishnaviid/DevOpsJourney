# 🐧 Linux Operating System 

Welcome to my DevOps learning journey! This repository documents my foundational understanding of the **Linux Operating System**—a crucial part of modern DevOps and cloud environments.

---

## 📌 What is an Operating System?

An **Operating System (OS)** acts as an interface between computer hardware and the user. It manages system resources like memory, processes, hardware devices, and files while enabling user interaction and application execution.

---

## 🧩 Components of an Operating System

### 1. Kernel  
The **kernel** is the core of the OS, managing:
- Process and memory handling  
- Device I/O operations  
- File system interactions  

Linux uses a **monolithic kernel**, meaning the entire OS runs in kernel space for performance.

### 2. Shell  
The **shell** is the interface between users and the kernel.
- **Command-Line Shells** (e.g., Bash, Zsh)  
- **Graphical Shells** (e.g., GNOME, KDE)

Commands entered in the terminal are interpreted by the shell.

### 3. File System  
Linux uses a **hierarchical file system**, beginning with the root `/` directory and branching into structured subdirectories.

### 4. System Libraries  
System libraries allow programs to access hardware functions without directly communicating with the kernel.

### 5. System Utilities & Applications  
Essential OS tools that handle system management like file handling, user management, and monitoring.

---

## Introduction to Linux

**Linux** is a free, open-source, Unix-based OS that powers everything from smartphones to cloud servers. It’s loved in DevOps for its:

✅ Stability  
✅ Performance  
✅ Flexibility  
✅ Open-source nature  

---

## Why Linux is Essential for DevOps

- Highly customizable and open-source  
- Secure and reliable  
- Rich in CLI tools  
- Lightweight and cloud-native  
- Dominates server and cloud infrastructure

---

## Popular Linux Distributions

| Distribution     | Purpose                             |
|------------------|-------------------------------------|
| Ubuntu           | Beginner-friendly and versatile     |
| CentOS / Rocky   | Stable, enterprise-grade systems    |
| Debian           | Server-focused and highly stable    |
| Kali Linux       | Security testing and penetration    |
| Fedora           | Cutting-edge and developer-centric  |

---

## Setting Up Linux on AWS EC2

To practice hands-on Linux skills in the cloud:

### Steps:
1. Create an AWS account  
2. Go to **EC2 → Launch Instance**  
3. Select **Amazon Linux AMI**  
4. Choose **t2.micro** (Free tier)  
5. Configure security group → Enable **port 22 (SSH)**  
6. Download the `.pem` key and launch the instance  

### 🔗 Connect via SSH:
ssh -i "your-key.pem" ec2-user@<EC2-Public-IP>




