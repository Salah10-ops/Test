# Complete DevOps Pipeline: Redis-Backed Python Counter App

## Project Overview

This project implements a full DevOps pipeline for a Python application backed by Redis.  
It covers Infrastructure as Code (Terraform), Configuration Management (Ansible), Containerization (Docker), Orchestration (Kubernetes on EKS), CI/CD (Jenkins), and Monitoring (Prometheus + Grafana).

## Prerequisites

Before you start, install the following tools:

- [Terraform](https://www.terraform.io/downloads.html)
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- [Docker](https://docs.docker.com/get-docker/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/)
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- [eksctl](https://eksctl.io/introduction/installation/)
- A GitHub Account
- An AWS Account

## Clone the Repository

```bash
git clone <your-github-repo-url>
cd <repo-name>

## 2. Configure AWS CLI

You need to configure the AWS CLI with your AWS credentials. Run the following command and provide your AWS access key, secret key, and region when prompted:

bash
Copy
Edit
aws configure
You’ll be asked to enter the following details:

AWS Access Key ID: Your AWS access key (you can generate this in the AWS console under IAM).

AWS Secret Access Key: Your AWS secret key (generated in IAM).

Default region name: Choose us-east-1 or your preferred region.

Default output format: You can leave this as json.

Additionally, ensure that your environment variables for AWS are set:

bash
Copy
Edit
export AWS_ACCESS_KEY_ID="your_access_key"
export AWS_SECRET_ACCESS_KEY="your_secret_key"
export AWS_REGION="us-east-1"
You can also use an .env file if you prefer not to set them manually every time.


