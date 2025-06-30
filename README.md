![Second_project](https://github.com/user-attachments/assets/4947c0c8-2f0e-4c32-92ee-7498f7bc50f2)
# CI/CD Project

This project demonstrates a full CI/CD pipeline with AWS, GitHub, Jenkins, Docker, Kubernetes, and Terraform.

## Structure
- terraform-infra: Terraform code to provision AWS infra
- jenkins: Jenkins Docker image and plugins
- registry: Private Docker registry
- microservices/user-service: Example Node.js service with Dockerfile, K8s manifests, and Jenkinsfile

Project Architecture
project-root/
│
├── terraform-infra/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│
├── jenkins/
│   ├── Dockerfile
│   ├── jenkins_home/
│   └── plugins.txt
│
├── registry/
│   ├── docker-compose.yml
│
├── microservices/
│   ├── user-service/
│   │   ├── app.py / index.js / main.java  # your app
│   │   ├── Dockerfile
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   └── Jenkinsfile
│   ├── order-service/ ...
│   └── catalog-service/ ...
│
└── README.md
Tech_Stack
| Tool                 | Purpose                 |
| -------------------- | ----------------------- |
| **AWS**              | Cloud infrastructure    |
| **GitHub**           | Source code repository  |
| **Jenkins**          | CI/CD pipeline          |
| **Docker**           | Containerization        |
| **Kubernetes (EKS)** | Container orchestration |
| **Terraform**        | Infrastructure as Code  |

Architecture daigram
(https://github.com/user-attachments/assets/0ed788f3-642f-46dd-a053-3134e715a90c)

