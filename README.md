# Python Tilt Cluster (Kubernetes + Docker + Tilt)

This project allows you to develop a JavaScript (Node.js) application directly in a Kubernetes cluster with DevSpace.

This project allows you to develop a Python application locally while automatically deploying it to a Kubernetes cluster with Tilt.

---

## 🚀 Prerequisites

Before you start, make sure you have installed:

- Docker
- Kubernetes (`kubectl` configured)
- Tilt
- Python 3.8+
- kind (optional but recommended)
- A working Kubernetes cluster
  
---

## 📦 Installation

### 1. Clone the project

```bash
git clone https://github.com/NizmoDev/Tilt.git
```

```bash
cd Tilt
```

---

### 2. Create the Kubernetes cluster

```bash
kind create cluster --name tilt-demo
```

---

### 3. Check the cluster

```bash
kubectl cluster-info
```

```bash
kubectl get nodes
```

---

### 4. 📦 Install Tilt

```bash
iex ((new-object net.webclient).DownloadString('https://raw.githubusercontent.com/tilt-dev/tilt/master/scripts/install.ps1'))
```

---

## ⚙️ Run the project with Tilt

### 1. Start Tilt

```bash
tilt up
```

---

## 🌐 Access the application

Open in the browser:

```text
http://localhost:10350/
```

---

## 🔄 Development workflow

Tilt handles the full CI/CD loop locally:

Detect file changes
Rebuild Docker image
Push image to local cluster
Redeploy Kubernetes manifests

---

## 🛑 Stop Tilt

```bash
tilt down
```

---

## 🧪 Useful commands

```bash
kubectl get pods
```

```bash
kubectl get deployments
```

```bash
kubectl get svc
```

```bash
tilt up
```

```bash
tilt down
```

```bash
devspace logs
```

```bash
docker ps
```

```bash
docker ps
```

---

## 📚 Tech stack

- Python
- Flask
- Kubernetes
- Docker
- Tilt
- kind
