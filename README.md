# Python Tilt Cluster (Kubernetes + Docker + Tilt)

Ce projet permet de développer une application JavaScript (Node.js) directement dans un cluster Kubernetes grâce à DevSpace.

Ce projet permet de développer une application Python localement tout en la déployant automatiquement dans un cluster Kubernetes grâce à Tilt.

---

## 🚀 Prérequis

Avant de commencer, assure-toi d’avoir installé :

- Docker
- Kubernetes (kubectl configuré)
- Tilt
- Python 3.8+
- kind (optionnel mais recommandé)
- Un cluster Kubernetes fonctionnel
  
---

## 📦 Installation

### 1. Cloner le projet

```bash
git clone https://github.com/NizmoDev/Tilt.git
```

```bash
cd Tilt
```

---

### 2. Créer le cluster Kubernetes

```bash
kind create cluster --name tilt-demo
```

---

### 3. Vérifier le cluster

```bash
kubectl cluster-info
```

```bash
kubectl get nodes
```

---

### 4. 📦 Installer Tilt

```bash
iex ((new-object net.webclient).DownloadString('https://raw.githubusercontent.com/tilt-dev/tilt/master/scripts/install.ps1'))
```

---

## ⚙️ Lancer le projet avec Tilt

### 1. Démarrer Tilt

```bash
tilt up
```

---

## 🌐 Accès à l’application

Ouvrir dans le navigateur :

```text
http://localhost:10350/
```

---

## 🔄 Workflow de développement

Tilt handles the full CI/CD loop locally:

Detect file changes
Rebuild Docker image
Push image to local cluster
Redeploy Kubernetes manifests

---

## 🛑 Arrêter Tilt

```bash
tilt down
```

---

## 🧪 Commandes utiles

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
