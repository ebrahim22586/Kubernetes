# Kubernetes Deployment on AWS

This project demonstrates deploying a scalable application on AWS using Kubernetes. The infrastructure leverages Amazon EKS (Elastic Kubernetes Service) for container orchestration, ECR (Elastic Container Registry) for image storage, EC2 instances as worker nodes, VPC (Virtual Private Cloud) for networking, ELB (Elastic Load Balancing) for traffic distribution, and Route53 for DNS management.

## Project Overview

This setup provisions a Kubernetes cluster on AWS, deploys a sample application, and configures networking and DNS services. The architecture enables high availability, scalability, and secure communication between services.

### Services Used

- **ECR (Elastic Container Registry)**: Stores Docker images for the application.
- **EKS (Elastic Kubernetes Service)**: Manages the Kubernetes control plane.
- **EC2 (Elastic Compute Cloud)**: Hosts worker nodes that run Kubernetes pods.
- **VPC (Virtual Private Cloud)**: Creates a network environment for Kubernetes, including private and public subnets.
- **ELB (Elastic Load Balancer)**: Manages incoming traffic and routes it to Kubernetes services.
- **Route53**: Provides DNS routing for the application domain.

## Prerequisites

- AWS CLI configured with IAM permissions to access ECR, EKS, EC2, VPC, ELB, and Route53.
- kubectl CLI installed and configured.
- eksctl CLI installed to simplify EKS setup.
- Docker for building images.

## Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-repo/k8s-aws-deployment.git
cd k8s-aws-deployment
