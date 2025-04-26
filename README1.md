# DevOps Pipeline for Redis-Backed Python Counter App

## Overview

This project demonstrates a complete DevOps pipeline setup for a Redis-backed Python counter application. It includes:
- Infrastructure provisioning using **Terraform**.
- Configuration management using **Ansible**.
- Containerization using **Docker**.
- Orchestration using **Kubernetes** (EKS).
- CI/CD pipeline setup with **Jenkins**.
- Monitoring using **Prometheus** and **Grafana**.

This guide walks you through the entire process of setting up the project from scratch.

---

## Prerequisites

Before you start, make sure you have the following tools installed:

- [Terraform](https://www.terraform.io/downloads.html) – For provisioning infrastructure.
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) – For configuration management.
- [Docker](https://docs.docker.com/get-docker/) – For building and running containers.
- [kubectl](https://kubernetes.io/docs/tasks/tools/) – To interact with Kubernetes clusters.
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) – To manage AWS resources.
- [eksctl](https://eksctl.io/introduction/installation/) – For creating and managing EKS clusters.
- **GitHub Account** – To clone the repository and manage CI/CD pipelines.

---

## Setup Instructions

### 1. Clone the Repository

Start by cloning the repository to your local machine:

```bash
git clone git@github.com:Salah10-ops
cd graduation_project
```

### 2. Configure AWS CLI

We need to configure the AWS CLI with the AWS credentials. Run the following command and provide your AWS access key, secret key, and region when prompted:

```bash

aws configure

```

1. AWS Access Key ID: Your AWS access key (you can generate this in the AWS console under IAM).
2. AWS Secret Access Key: Your AWS secret key (generated in IAM).
3. Default region name: Choose us-east-1 or your preferred region.
4. Default output format: You can leave this as json.


---

## Infrastructure Setup

### Initialize and Apply Terraform

Navigate to the Terraform folder: 

```bash  
cd terraform/
terraform init
terraform plan
terraform apply
```
This will create the following resources:

1. EKS Cluster for container orchestration.
2. VPC, Subnets, and Networking resources.
3. EC2 Instance for Jenkins.
4. IAM Roles and Policies for AWS access.
