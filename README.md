# 📊 Task 7: Monitor System Resources Using Netdata

## 📌 Internship Task Overview

This project is part of the **DevOps Internship** program. The goal is to install and run **Netdata** — an open-source, lightweight monitoring tool — using Docker, and visualize real-time system resource metrics via its built-in web dashboard.

---

## 🎯 Objective

> Install Netdata using Docker and monitor system performance, including CPU, memory, disk, and Docker container metrics through a real-time web dashboard.

---

## 🛠 Tools & Technologies

| Tool        | Purpose                              |
|-------------|--------------------------------------|
| **Netdata** | System monitoring dashboard          |
| **Docker**  | Containerizing and running Netdata   |
| **Web Browser** | To access the Netdata dashboard |
| **PowerShell / Terminal** | For command-line operations |

---

## 🚀 Step-by-Step Instructions

### ✅ Step 1: Install Docker

If Docker is not already installed:

- Download Docker from [https://www.docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop)
- Install it based on your OS (Windows, Mac, or Linux)
- After installation, confirm Docker is working:
  ```bash
  docker --version

###  ✅ Step 2: Run Netdata using Docker
Run this command in terminal (PowerShell, CMD, or Linux shell):

```bash

docker run -d --name=netdata -p 19999:19999 netdata/netdata
```
✔️ This does the following:

Pulls the official Netdata Docker image (if not already available)

Starts a container named netdata

Maps container’s port 19999 to your local 19999 for browser access

### ✅ Step 3: Access the Netdata Dashboard
Once the container is running:

Open your browser
```bash

Visit: http://localhost:19999
```

✔️ You’ll now see an interactive, real-time dashboard with metrics like:

CPU usage

RAM and swap

Disk I/O

Network activity

Docker container health

### ✅ Step 4: Explore Features
Navigate through the dashboard to explore:

Alerts section

Individual chart panels

Docker metrics (if you're running other containers)

Logs via /var/log/netdata (if using full install, optional in Docker)

### ✅ Step 5: Stop/Remove the Container (Optional)
To stop Netdata:

```bash
docker stop netdata
```
To delete it:

```bash

docker rm netdata
```
### 📂 Folder Structure

internship-task-7/
├── screenshots/
│   └── netdata-dashboard.png
├── README.md

### 📷 Screenshot
Network Chart
![network metrics](https://github.com/user-attachments/assets/b737bc86-29e0-4515-841f-7cc2536a1efd)
Memory Chart
![memory charts](https://github.com/user-attachments/assets/12cdca57-3d37-4762-9c93-184ed6d5389d)
Login Dashboard
![login dashboard](https://github.com/user-attachments/assets/2fa20f71-2dd5-4646-8c0d-a3583f4d10e8)
Compute Chart
![compute metrics](https://github.com/user-attachments/assets/615af5ee-e2c7-4fa1-8145-c5669c5b9d6f)


### ✅ Key Learnings

Setup and ran a Docker container

Monitored system resource metrics in real-time

Understood performance KPIs like CPU, RAM, and I/O load

Gained experience with lightweight monitoring tools for DevOps/Analytics


