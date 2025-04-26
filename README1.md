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


---

## Setup Instructions

### 1. Clone the Repository

Start by cloning the repository to your local machine:

```bash
git clone git@github.com:Salah10-ops
cd graduation_project


### 2. Configure AWS CLI

You need to configure the AWS CLI with your AWS credentials. Run the following command and provide your AWS access key, secret key, and region when prompted:

bash
