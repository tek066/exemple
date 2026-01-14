# DevOps Mini Project – Automated Web Server Deployment

## 📌 Overview
This project demonstrates a DevOps-oriented approach to automating the installation and configuration of a web server on Linux using Bash scripting.

The goal is to deploy a fully functional **Nginx web server** in a **repeatable, reliable and idempotent** way.

---

## 🎯 Objectives
- Automate web server installation
- Apply DevOps best practices
- Ensure service reliability
- Validate deployment automatically

---

## 🛠️ Technologies Used
- Linux (Ubuntu/Debian)
- Bash scripting
- systemd
- Nginx
- Git / GitHub

---

## 🚀 What the Script Does
The script performs the following actions:

1. Verifies root privileges
2. Installs Nginx if not already installed
3. Enables and starts the Nginx service
4. Deploys a static HTML page
5. Verifies service availability using `curl`
6. Logs all actions with timestamps
7. Can be executed multiple times safely (idempotent)

---

## ▶️ How to Run
```bash
sudo bash install_nginx.sh

