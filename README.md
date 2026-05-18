# 🚀 Dockerized Professional Web Server

## Project Overview
Professional web application using Docker and Nginx, deployed on Ubuntu EC2.

This project demonstrates containerization, cloud deployment, Linux administration, and web hosting using Docker and Nginx.

---

## 🛠 Tech Stack

- Docker
- Nginx
- Ubuntu (AWS EC2)
- HTML/CSS
- Git & GitHub

---

## ✨ Features

- Fully containerized web application
- High-performance Nginx server
- Cloud deployment on AWS EC2
- Easy container lifecycle management
- Basic scaling support
- Responsive professional portfolio website

---

## 📦 Deployment

### 1. Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

---

### 2. Go to Project Directory

```bash
cd YOUR_REPOSITORY
```

---

### 3. Build Docker Image

```bash
docker build -t my-docker-web .
```

---

### 4. Run Docker Container

```bash
docker run -d -p 80:80 --name docker-web-container my-docker-web
```

---

### 5. Verify Running Containers

```bash
docker ps
```

---

### 6. Access Website

Open browser:

```bash
http://EC2_PUBLIC_IP
```

---

## 📁 Project Structure

```bash
.
├── Dockerfile
├── index.html
└── README.md
```

---

## 🐳 Dockerfile

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
```

---

## ☁️ AWS EC2 Setup

- Ubuntu EC2 Instance
- Port 80 allowed in Security Group
- Docker installed on server

---

## 📚 DevOps Concepts Used

- Docker Containerization
- Web Server Deployment
- Linux Administration
- AWS Cloud Hosting
- GitHub Version Control
- Networking & Port Mapping

---

## 👨‍💻 Author

Firdose Shaikh  
AWS Cloud & DevOps Engineer
