![Terraform](https://img.shields.io/badge/Terraform-1.14.x-623CE4?logo=terraform)
![AWS](https://img.shields.io/badge/AWS-EKS-orange?logo=amazonaws)
![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-326CE5?logo=kubernetes)
![License](https://img.shields.io/badge/License-EPL--2.0-blue)
![IaC](https://img.shields.io/badge/Infrastructure-as-Code-success)


🚀 Terraform-based EKS CI/CD Infrastructure
📌 Project Overview

This project provisions a production-ready AWS EKS infrastructure using Terraform, designed to support a complete CI/CD pipeline for a containerized application.

The infrastructure is modular, reusable, and follows Infrastructure as Code (IaC) best practices, making it suitable for real-world DevOps workflows and interviews.

🚀 Terraform-based EKS CI/CD Infrastructure
📌 Project Overview

This project provisions a production-ready AWS EKS infrastructure using Terraform, designed to support a complete CI/CD pipeline for a containerized application.

The infrastructure is modular, reusable, and follows Infrastructure as Code (IaC) best practices, making it suitable for real-world DevOps workflows and interviews.

terraform/
├── backend.tf          # Remote state backend (S3)
├── provider.tf         # AWS provider configuration
├── versions.tf         # Terraform & provider version locks
├── variables.tf        # Input variables
├── terraform.tfvars    # Environment-specific values
├── vpc.tf              # Networking (VPC, subnets, routing)
├── iam.tf              # IAM roles & policies
├── eks.tf              # EKS cluster & node groups
├── ecr.tf              # ECR repositories
├── ec2.tf              # Optional EC2 instances (e.g., Jenkins)
├── outputs.tf          # Useful outputs
└── modules/            # Reusable Terraform modules
    ├── vpc/
    ├── iam/
    ├── eks/
    └── ec2/

⚙️ Prerequisites

Terraform >= 1.4

AWS CLI v2

AWS account with sufficient IAM permissions

Git

WSL / Linux / macOS environment


🔄 CI/CD Integration (Planned)

Jenkins pipeline for build & deploy

Docker image build & push to ECR

Kubernetes deployment via manifests

Auto-scaling using HPA

Monitoring with Prometheus & Grafana

Logging via CloudWatch / Fluentd

👤 Author

Anandan S
DevOps | Kubernetes | Terraform | AWS
GitHub: https://github.com/unixanand


