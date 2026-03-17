# 🖥️ VirtualBox & Ubuntu 22.04 Installation Guide

### Course: Networking
### Name: Umutoniwase Benefice 
### ID: 27368

## 📌 Project Overview

This project documents the step-by-step process of downloading and installing VirtualBox and setting up Ubuntu 22.04 LTS on a virtual machine.

---

## 🚀 Step 1: Download & Install VirtualBox

### 1. Visit Official Website

Go to: https://www.virtualbox.org/

### 2. Download VirtualBox

* Click on **Downloads**
* Select your OS (Windows / macOS / Linux)

### 3. Install VirtualBox

* Open the downloaded file
* Follow installation steps:

  * Click **Next**
  * Choose installation location
  * Install required dependencies
  * Click **Install**
* Finish installation

---

## 🐧 Step 2: Download Ubuntu 22.04 LTS

### 1. Visit Ubuntu Website

Go to: https://ubuntu.com/download/desktop

### 2. Download ISO File

* Select **Ubuntu 22.04 LTS**
* Click **Download**
* Save the `.iso` file

---

## ⚙️ Step 3: Create Virtual Machine

### 1. Open VirtualBox

* Click **New**

### 2. Configure VM

* Name: Ubuntu 22.04
* Type: Linux
* Version: Ubuntu (64-bit)

### 3. Allocate Resources

* RAM: Minimum 2GB (Recommended 4GB+)
* CPU: 2 cores (if available)

### 4. Create Virtual Hard Disk

* Select **VDI (VirtualBox Disk Image)**
* Storage: Dynamically allocated
* Size: At least 20GB

---

## 💿 Step 4: Install Ubuntu

### 1. Attach ISO File

* Select your VM → Click **Settings**
* Go to **Storage**
* Add Ubuntu ISO file

### 2. Start VM

* Click **Start**
* Ubuntu installer will launch

### 3. Installation Steps

* Select language
* Choose **Install Ubuntu**
* Select keyboard layout
* Choose installation type:

  * Normal Installation
* Create user:

  * Username
  * Password

### 4. Finish Installation

* Restart VM
* Remove ISO when prompted

---

## 🧠 Concepts Covered

* Virtualization
* Hypervisor (VirtualBox)
* ISO Images
* Operating System Installation
* Resource Allocation (RAM, CPU, Storage)
* Virtual Machines (VMs)
* Disk Types (Dynamic vs Fixed)
* Linux Basics

---
