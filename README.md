🚀 SnapDFY DevOps CI/CD Pipeline

A production-grade, end-to-end CI/CD pipeline designed to automate the build, packaging, and deployment of a containerized web application using modern DevOps practices and AWS services.

This project demonstrates how to integrate GitHub, Jenkins, Docker, AWS ECR, and EC2 to achieve fully automated deployments with zero manual intervention.

🧠 Overview

The pipeline is triggered automatically on every code push to GitHub via webhooks. Jenkins orchestrates the entire workflow — building the Docker image, pushing it to AWS Elastic Container Registry (ECR), and deploying the latest version to an EC2 instance via secure SSH.

The application is served through Nginx with HTTPS enabled (Let’s Encrypt), making the setup production-ready.

⚙️ Key Features

🔄 Automated CI/CD Pipeline triggered on every Git push
🐳 Dockerized Application for consistent environments
☁️ AWS ECR Integration for secure image storage
🚀 Automated Deployment on EC2 using SSH
🔐 HTTPS Enabled using Nginx + Certbot
🔁 Auto Container Restart on instance reboot
⚡ Zero Manual Deployment Effort


🏗️ Architecture

GitHub → Jenkins → Docker Build → AWS ECR → EC2 (Docker) → Nginx → Live Domain



🛠️ Tech Stack

Backend: Python (Flask)
CI/CD: Jenkins
Containerization: Docker
Cloud: AWS (EC2, ECR)
Web Server: Nginx
Security: Let’s Encrypt SSL
Version Control: GitHub


🚀 Deployment Workflow

Developer pushes code to GitHub
GitHub webhook triggers Jenkins pipeline
Jenkins builds Docker image
Image is pushed to AWS ECR
Jenkins connects to EC2 via SSH
Latest image is pulled and container is redeployed
Application is live with updated changes

🌐 Live Application

👉 http://snapdfy.in




📌 Key Learnings

Designing real-world CI/CD pipelines
Docker image lifecycle management
Secure AWS deployments using IAM & ECR
SSH-based remote automation
Production-ready infrastructure setup
🔮 Future Enhancements
Blue-Green / Canary Deployments
Kubernetes (EKS) migration
Monitoring (Prometheus + Grafana)
Auto Scaling with Load Balancer
Security Scanning (Trivy, SonarQube, OWASP)



👨‍💻 Author

Kushagra Sharma
Cloud & DevOps Engineer