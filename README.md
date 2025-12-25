#  3-Tier DevOps Application using Docker, Kubernetes & GitHub Actions

This project demonstrates a **complete 3-tier DevOps application** deployed on **AWS EC2** using **Docker**, **Kubernetes (k3s)**, and **GitHub Actions CI/CD**.

The application follows **real-world DevOps practices** including containerization, orchestration, CI/CD automation, and reverse proxy configuration.

---

## 🧱 Architecture Overview

Browser
|
| NodePort
v
Frontend (Nginx)
|
| /api (Reverse Proxy)
v
Backend (Flask)

---

## 🛠️ Tech Stack

- **Cloud**: AWS EC2 (Free Tier)
- **Containerization**: Docker
- **Orchestration**: Kubernetes (k3s)
- **CI/CD**: GitHub Actions
- **Frontend**: Nginx
- **Backend**: Flask (Python)

---

## 📁 Project Structure

devops-3tier-project/
├── backend/
│ ├── app.py
│ └── Dockerfile
├── frontend/
│ ├── index.html
│ ├── nginx.conf
│ └── Dockerfile
├── k8s/
│ ├── backend.yaml
│ └── frontend.yaml
└── .github/
└── workflows/
└── cicd.yml


---

## ⚙️ Application Flow

1. User accesses the application via browser  
2. Request reaches **Frontend (Nginx)** through NodePort  
3. Clicking **Call Backend** sends request to `/api`  
4. Nginx reverse proxy forwards the request to **Backend service**  
5. Backend responds with message  
6. Response is displayed on UI  

---

## 🔄 CI/CD Pipeline

- Triggered on every push to `main`
- Builds Docker images for frontend & backend
- Pushes images to Docker Hub
- Deploys updated containers to Kubernetes on EC2

---

## 🚀 Deployment Summary

1. AWS EC2 created (Free Tier)
2. Docker & Kubernetes (k3s) installed
3. Kubernetes manifests created
4. Nginx reverse proxy configured
5. GitHub Actions CI/CD implemented
6. Application deployed on Kubernetes

---

## 🌐 Application Access

http://<EC2_PUBLIC_IP>:30007


### Final Output

3 Tier DevOps App
Call Backend
Hello from Backend


---

## 🧠 Key DevOps Learnings

- Kubernetes service-to-service communication
- Reverse proxy using Nginx
- CI/CD automation with GitHub Actions
- Cloud deployment on AWS Free Tier
- Real-world Kubernetes troubleshooting

---

## 🙌 Author

**Akshatha**  
DevOps Enthusiast
