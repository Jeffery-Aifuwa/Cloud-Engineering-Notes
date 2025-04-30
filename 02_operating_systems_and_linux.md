# Operating Systems (OS)

## What is an Operating System?

An **Operating System (OS)** is the middleman between users and computer hardware. It manages system resources and simplifies user interaction with computers.

---

## Functions of an OS

- **File Management** – Organizing and handling files.
- **Memory Management** – Allocating system memory efficiently.
- **Process Scheduling** – Deciding which programs run and when.
- **Device Management** – Connecting and controlling hardware components.
- **User Management** – Handling permissions and security for multiple users.

---

## Popular Operating Systems

- Windows  
- macOS  
- Linux  
- Android  
- iOS  
- Chrome OS  

---

## Introduction to Linux

**Linux** is an open-source OS, meaning anyone can modify and share it. Developers have created many distributions (distros), such as:

- Ubuntu  
- Fedora  
- Debian  

**Cool Fact:** You can create your own Linux OS by cloning an existing version and customizing it — though it requires deep technical knowledge.

---

## Why Focus on Linux in Cloud Engineering?

- ✅ **Free & Open-Source** – No licensing fees, fully customizable.  
- ✅ **Stable & Secure** – Preferred for servers and cloud platforms.  
- ✅ **Command Line Power** – Many cloud tasks use the Linux terminal.  
- ✅ **Lightweight & Efficient** – Ideal for cloud environments with minimal hardware.

---

## Linux Kernel: The Heart of the OS

The **Linux kernel** is the core of the OS, managing critical tasks between hardware and software.

### Four Main Jobs of the Linux Kernel (with Examples):

1. **Process Management**  
   🧠 Controls which programs run and for how long.  
   *Example:* Running multiple apps like a browser and music player smoothly.

2. **Memory Management**  
   📦 Manages RAM usage to prevent crashes.  
   *Example:* Ensures each browser tab has enough memory.

3. **Device Management**  
   🔌 Links hardware (keyboard, mouse, storage) with software.  
   *Example:* Your keystrokes show instantly on screen.

4. **File System Management**  
   📁 Organizes and retrieves files.  
   *Example:* Saves documents efficiently and keeps them accessible.

---

### Analogy:
- **OS** = Car 🚗 — what you see and interact with.  
- **Kernel** = Engine 🏎️ — does the hidden heavy lifting.

---

## Virtualization and Linux Setup

I installed:

- **VirtualBox**
- **Ubuntu**
- **Vagrant**
- **Ubuntu Focal 64** (via Git Bash)

### Vagrant Setup in Terminal

1. **Initialize Vagrant in a directory**
   ```bash
   vagrant init ubuntu/focal64
   ```
   Creates a `Vagrantfile` in the current directory.

2. **Start and provision the virtual machine**
   ```bash
   vagrant up
   ```
   Downloads and starts the Ubuntu Focal 64 box.

3. **Access the virtual machine**
   ```bash
   vagrant ssh
   ```
   SSH into the running virtual machine.

---

> 🚀 This forms the foundation for hands-on Linux experience in cloud environments.
