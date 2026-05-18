# Professional DevOps Portfolio HTML - Dockerized Web Server Project

## Project Overview

This project demonstrates how to deploy a professional HTML portfolio website using Docker and Nginx on an Ubuntu EC2 instance in AWS Cloud.

The application is containerized using Docker and served through the Nginx web server. The project showcases practical DevOps concepts including cloud deployment, Linux administration, Docker containerization, networking, and web hosting.

---

## Technologies Used

- AWS EC2
- Ubuntu Linux
- Docker
- Nginx
- Git & GitHub
- HTML & CSS

---

## Project Architecture

User Browser
      ↓
AWS EC2 Instance
      ↓
Docker Container
      ↓
Nginx Web Server
      ↓
Portfolio Website

---

## Features

- Dockerized static website deployment
- Nginx web server configuration
- Cloud deployment on AWS EC2
- Container-based application hosting
- Responsive professional portfolio website
- GitHub version control integration

---

## Prerequisites

Before starting:

- AWS Account
- Ubuntu EC2 Instance
- Docker installed
- Git installed

---

## Step 1 — Connect to EC2

```bash
ssh -i key.pem ubuntu@YOUR_PUBLIC_IP
```

---

## Step 2 — Install Docker

```bash
sudo apt update
sudo apt install docker.io -y
```

Start Docker:

```bash
sudo systemctl start docker
sudo systemctl enable docker
```

---

## Step 3 — Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

Go to project directory:

```bash
cd YOUR_REPOSITORY
```

---

## Step 4 — Build Docker Image

```bash
docker build -t portfolio-webserver .
```

---

## Step 5 — Run Docker Container

```bash
docker run -d -p 80:80 --name portfolio-container portfolio-webserver
```

---

## Step 6 — Verify Running Container

```bash
docker ps
```

---

## Step 7 — Access Website

Open browser:

```bash
http://YOUR_PUBLIC_IP
```

---

## Dockerfile Used

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
```

---

## DevOps Concepts Demonstrated

- Cloud Infrastructure Deployment
- Linux Server Administration
- Docker Containerization
- Web Server Management
- Application Hosting
- Networking & Port Mapping
- GitHub Version Control

---

## Future Improvements

- Add Jenkins CI/CD Pipeline
- HTTPS SSL Configuration
- Kubernetes Deployment
- Monitoring with Prometheus & Grafana
- Domain Name Integration

---

## Author

Firdose Shaikh

AWS Cloud & DevOps Engineer

