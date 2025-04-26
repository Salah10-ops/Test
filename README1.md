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
