# SETUP.md
### Local Development Setup Guide

This document explains how to set up your development environment for **AI-Resilience-Orchestrator**.

---

## 1. Requirements

Before starting, ensure you have the following installed:

- **Git**
- **Docker & Docker Compose**
- **Python 3.10+**
- (Optional) **Go** or **Rust**
- (Optional) **Minikube** or local Kubernetes cluster
- **VS Code** or any IDE of your choice

---

## 2. Clone the Repository

```bash
git clone https://github.com/katumbasudais/AI-Resilience-Orchestrator.git
cd AI-Resilience-Orchestrator
```

---

## 3. Python Setup (AI Controller & Detection Agent)

### Create a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate     # Linux/macOS
venv\Scripts\activate        # Windows
```

### Install dependencies:
```bash
pip install -r requirements.txt
```

---

## 4. Run the Simulation (Docker Prototype)

```bash
docker compose up --build
```

This launches:

- **Detection Agent**
- **AI Controller**
- **Deployment Engine**
- **Fake Kubernetes cluster simulator**

---

## 5. Kubernetes Optional Setup (for advanced devs)

### Start Minikube:
```bash
minikube start
```

### Verify:
```bash
kubectl get nodes
```

---

## 6. Linting & Formatting

### Python:
```bash
black .
flake8 .
```

### Go:
```bash
gofmt -w .
```

### Rust:
```bash
cargo fmt
```

---

You're ready to begin contributing 🚀  
For contribution rules, see **CONTRIBUTING.md**.
