# Automated Cloud Deployment with Terraform, Ansible, and Docker

## Overview
This repository contains code for automating the deployment of a Dockerized Nginx server on an AWS EC2 instance, using Terraform, Ansible, and GitHub Actions CI/CD pipeline.

## Project Structure
- **main.tf** - Terraform configuration to provision an EC2 instance on AWS.
- **deploy.yml** - Ansible playbook to install Docker, set up the Nginx container, and serve a custom index file.
- **ci-cd.yml** - GitHub Actions workflow for CI/CD pipeline, automating infrastructure setup and configuration deployment.

## Getting Started
### Prerequisites
- AWS Account with `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`, and `AWS_REGION` set in GitHub Secrets.
- SSH Key (`my-key-pair.pem`) added in GitHub Secrets for SSH access.

### Usage
1. Clone the repository.
2. Push changes to `main` branch to trigger the pipeline.
3. Check `vm_ip.txt` for the deployed instance IP.

## Security
- AWS credentials and SSH keys are securely managed using GitHub Secrets.
