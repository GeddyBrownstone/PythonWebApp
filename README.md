# PythonWebApp
A Django-based Python web application deployed on Kubernetes using a modern DevOps toolchain (Docker, Kubernetes, and Nginx). Built to gain real-world experience with cloud-native architecture, CI/CD pipelines, and scalable application deployment.

![screenshot](https://github.com/GeddyBrownstone/PythonWebApp/blob/main/Screenshot.png)

Python Web App — Django + Gunicorn + Nginx + Kubernetes (K3s)

This project is a fully containerized, production-grade web application built with Django, served with Gunicorn, proxied through Nginx, and deployed on a lightweight K3s Kubernetes cluster.

It demonstrates modern DevOps practices, multi-environment deployments (staging & production), CI/CD readiness, container orchestration, and clean application structure — making it an ideal example of a real-world web service.

For now, the application displays ASCII-styled greetings generated from user input, using server-side rendering and session handling.

Tech Stack
Backend

Django — Core web framework
Gunicorn — Python WSGI server
Pyfiglet — ASCII art rendering

Frontend
HTML + CSS (lightweight, Django templating)

Infrastructure
Docker — Multi-container build (Django/Gunicorn + Nginx)
Kubernetes (K3s) — Lightweight, production-ready cluster
Helm/Kubectl — Deployment management
ConfigMaps & Secrets — Environment and secure data separation
Sidecar Pattern — Nginx + Django in the same pod

Deployment Environments
Staging namespace
Production namespace
Independent configs, identical containers

Key Features
Fully containerized architecture
 - Both the backend and web server run as isolated containers using Docker.

Production-ready configuration
 - Gunicorn + Nginx & strict config separation for staging vs. production.

Kubernetes-native deployment
 - Used Deployments, Services, ConfigMaps, Secrets, and namespaces.

Sidecar pattern
 - Django and Nginx run in a single pod, simulating common production setups.

CI/CD-friendly
 - Repo structure, Dockerfile, and K8s manifests are organized for an easy transition into GitHub Actions or Jenkins.

This project was designed to demonstrate:

Cloud-native deployment skills
Kubernetes hands-on experience
Infrastructure-as-code practices
Container orchestration
Proper multi-environment architecture
Python + Django production-style setup
Build + deploy a complete full-stack web application
