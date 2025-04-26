# 🛠️ osTicket - Prerequisites and Installation Guide

This guide outlines the prerequisites and step-by-step installation process for setting up **osTicket**, an open-source help desk ticketing system, on a Windows environment using IIS.

## ✅ Environments and Technologies Used

- **Microsoft Azure** – Virtual Machines (Compute)
- **Windows 10 (21H2)** – Operating System
- **Remote Desktop Protocol (RDP)** – For VM access
- **Internet Information Services (IIS)** – Web Server
- **PHP** – Backend scripting language
- **MySQL** – Database engine
- **osTicket v1.x** – Help desk system

---

## 📋 Prerequisites

Ensure the following components are installed **before** proceeding with osTicket setup:

1. **Windows 10 (21H2)** VM or local machine  
2. **IIS (Internet Information Services)** with the following features:
   - CGI
   - Common HTTP Features
3. **PHP Manager for IIS**
4. **PHP**
5. **MySQL Server**

---

## 🚀 Installation Steps
![image](https://github.com/user-attachments/assets/14ad2d01-df00-4469-9997-c71e69b9a4ad)
### Step 1: Prepare the Environment
- Launch your Windows 10 VM or machine.
- Open `Server Manager > Manage > Add Roles and Features`.
- Install **Web Server (IIS)** and the required role services listed in prerequisites.

![image](https://github.com/user-attachments/assets/53bcb6ea-976e-41bd-a509-cf635df6a297)
### Step 2: Install PHP, ReWrite, Virtual Code
- Download and install PHP for Windows from the official PHP website.
- Configure PHP to work with IIS using **PHP Manager for IIS**.
- PHP will be responsible for backend scripting ... PHP will interact with MySQL to manage the database

![image](https://github.com/user-attachments/assets/b2bf8e24-8f69-4f10-a2eb-725fea2bb730)
### Step 3: Install MySQL
- Download and install MySQL and setup configuration
- Launch with username and password

![image](https://github.com/user-attachments/assets/2907f604-1af4-432f-bf73-b0bbf3b947b0)
### Step 4: Install osTicket & Launch osTicket
- Download and extract osTicket folder into upload folder in wwwroot
- rename upload folder to osTicket
- Enable osTicket extensions
- Rename ost-sampleconfig.php --> ost-config.php & assign new permissions

![image](https://github.com/user-attachments/assets/ed50c679-5daf-4c95-b5cc-bf3cd61a399c)
### Step 5: Install & Configure HeidiSQL
- Create new session with username and password from MySQL
- Connect to the session
- Create database for osTicket

![image](https://github.com/user-attachments/assets/97ddb775-2cef-4785-b612-eaec883926ea)
### Step 6: Login to osTicket
- Login using created username and password
