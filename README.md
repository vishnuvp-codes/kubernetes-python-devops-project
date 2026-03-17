
# Kubernetes Python DevOps Project

This project demonstrates how to deploy a **Python Flask application** using **Docker and Kubernetes**. The application is containerized with Docker and deployed to a Kubernetes cluster using Minikube.

---

## 🚀 Technologies Used

- Linux (Ubuntu)
- Docker
- Kubernetes (Minikube)
- Python Flask
- YAML (Kubernetes configuration)
- Git & GitHub

---

## 📦 Project Architecture

Python Flask Application  
↓  
Docker Container  
↓  
Kubernetes Deployment  
↓  
Kubernetes Pods  
↓  
Kubernetes Service (NodePort)  
↓  
Browser Access

---

## 📁 Project Structure

```

k8s-python-project
│
├── app.py
├── Dockerfile
├── deployment.yaml
├── service.yaml
└── README.md

````

---

## ⚙️ Application Code

### app.py

Simple Flask application that runs inside the container.

---

## 🐳 Docker Image Build

Build the Docker image:

```bash
docker build -t python-k8s-app .
````

Verify Docker image:

```bash
docker images
```

---

## ☸️ Kubernetes Deployment

Deploy the application:

```bash
kubectl apply -f deployment.yaml
```

Check running pods:

```bash
kubectl get pods
```

---

## 🌐 Expose Application

Create service:

```bash
kubectl apply -f service.yaml
```

Check services:

```bash
kubectl get svc
```

Access application:

```bash
minikube service python-service
```

---

## 📊 Key DevOps Concepts Demonstrated

* Containerization using Docker
* Kubernetes Deployment and Pod management
* Service exposure using NodePort
* Application scaling using replicas
* Infrastructure configuration using YAML

---

##  Learning Outcomes

This project helped me understand:

* Docker container creation
* Kubernetes architecture (Pods, Deployments, Services)
* Deploying applications in a Kubernetes cluster
* Basic DevOps workflow from development to deployment

---

##  Future Improvements

* CI/CD pipeline using GitHub Actions
* Kubernetes Ingress configuration
* Monitoring with Prometheus and Grafana
* Deploying to cloud platforms (AWS / GCP)

---

## 👩‍💻 Author

**Vishnupriya**
MCA Graduate | Linux | Docker | Kubernetes | DevOps 
