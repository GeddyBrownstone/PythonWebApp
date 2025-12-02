# PythonWebApp
A Django-based Python web application deployed on Kubernetes using a modern DevOps toolchain (Docker, Kubernetes (K3s), and Nginx). Cloud-native architecture, CI/CD pipelines, and scalable application deployment.

![screenshot](https://github.com/GeddyBrownstone/PythonWebApp/blob/main/Screenshot.png)

## Tech Stack

### Backend
- **Django** — Core web framework  
- **Gunicorn** — Python WSGI server  

### Frontend
- **HTML + CSS** — Lightweight, Django templating  

### Infrastructure
- **Docker** — Multi-container build (Django/Gunicorn + Nginx)  
- **Kubernetes (K3s)** — Lightweight, production-ready cluster  
- **Helm / kubectl** — Deployment management  
- **ConfigMaps & Secrets** — Environment and secure data separation  
- **Sidecar Pattern** — Nginx + Django in the same pod  

## Deployment Environments
- **Staging namespace**  
- **Production namespace**  
- Independent configs with identical containers  

## Key Features

- **Fully containerized architecture**  
  Both the backend and web server run as isolated containers using Docker.  

- **Production-ready configuration**  
  Gunicorn + Nginx with strict config separation for staging vs. production.  

- **Kubernetes-native deployment**  
  Utilizes Deployments, Services, ConfigMaps, Secrets, and namespaces.  

- **Sidecar pattern**  
  Django and Nginx run in a single pod, simulating common production setups.  
