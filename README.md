# 🚀 Go Web App CI/CD

A complete DevOps implementation project demonstrating end-to-end automation for a Golang web application. This project features containerization with multi-stage Docker builds, Kubernetes deployment, CI/CD pipelines using GitHub Actions, and Helm charts for environment management.

---

## 📌 Project Overview

This project transforms a simple Go web app into a production-ready deployment using modern DevOps practices. It covers:

- Local development  
- Containerization  
- Automated testing  
- CI/CD automation  
- Kubernetes orchestration  
- Secure, public access using Ingress & DNS

---

## ✨ Features

✅ **Multi-stage Docker Build** – Optimized, minimal, secure container images  
✅ **Kubernetes Deployment** – Manifests for Deployment, Service & Ingress  
✅ **CI/CD with GitHub Actions** – Automated build, test, and deploy  
✅ **Helm Charts** – Environment-specific deployments  
✅ **DockerHub Integration** – Push & pull container images  
✅ **Production-Ready Ingress & DNS Setup**

---

## 📋 Prerequisites

Make sure you have the following tools installed:

- [Go](https://golang.org/dl/) 1.22.x or higher  
- [Docker](https://www.docker.com/products/docker-desktop/)  
- [Kubernetes](https://kubernetes.io/) cluster (minikube/kind/EKS/etc.)  
- [Helm](https://helm.sh/) 3.x  
- `kubectl` CLI  
- Git & GitHub

---

## 🛠️ Quick Start

### 🔧 1. Clone and Run Locally

```bash
git clone https://github.com/rohittsinghh/go-web-app-cicd.git
cd go-web-app-cicd
go build -o main
./main
```
🔗 Visit [http://localhost:8080/courses](http://localhost:8080/courses) to view the app in your browser.
---
### 🐳 2. Build and Run with Docker
```bash
docker build -t rohittsinghh/go-web-app:latest .
docker run -p 8080:8080 rohittsinghh/go-web-app:latest
```
## 📊 CI/CD Pipeline Overview

The project includes a robust GitHub Actions pipeline with the following stages:

- **Build** – Compile the Go app  
- **Code Quality** – Run linters and formatters  
- **Push** – Push Docker image to DockerHub  
- **Helm Update** – Automatically update image tag in Helm Chart
---
## 🐳 Docker Registry Integration

Docker images stored on DockerHub:

![Docker Registry](Screenshot-From-2025-09-18-05-49-42.jpg)

Details:
- **Repository:** rohittsinghh/go-web-app
- **Image Size:** ~13MB (multi-stage build)
- **Architecture:** linux/amd64

---
## ⚙️ Helm Configuration

Helm charts provide flexibility for multiple environments:

![Helm Values](Screenshot-From-2025-09-18-05-50-55.jpg)
---

---

## 🌐 Application Demo

The deployed application home page:

![Application Homepage](Screenshot-From-2025-09-18-12-55-45.jpg)

Features:
- **Courses**: Zero to Hero DevOps topics
- **Overview & About**: Project context
- **Contact**: Ways to reach out

---

## 🚀 Deployment

### With kubectl
```bash
kubectl apply -f k8s/
kubectl get pods
kubectl get svc
```
---
### With Helm
```bash
helm install go-web-app ./go-web-app-chart
```

---

## 🔒 Security

- Distroless base images
- Non-root user
- Resource/configuration limits
- Network policies support

---

## 🔗 Resources

- [Reference Video Tutorial](https://youtu.be/HGu9sgoHaJ0)
- [DockerHub: rohittsinghh/go-web-app](https://hub.docker.com/r/rohittsinghh/go-web-app)
- [GitHub Actions Docs](https://docs.github.com/actions)
- [Kubernetes Docs](https://kubernetes.io/docs/)
- [Helm Docs](https://helm.sh/docs/)

---

## 🤝 Contributing

1. Fork repo
2. Create feature branch
3. Commit changes
4. Push & open PR

---

## 📝 License

MIT — see [LICENSE](LICENSE).

---

**Star this repo if you found it helpful!**



