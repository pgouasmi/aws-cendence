# Transcendence Infrastructure Project

## Overview

This project documents my journey into learning modern cloud infrastructure practices through the implementation of a microservices-based application. I created this project specifically to gain hands-on experience with Infrastructure as Code (IaC), CI/CD pipelines, and AWS cloud services.

## Learning Objectives

Throughout this project, I focused on:

- **Infrastructure as Code**: Learning Terraform to define and provision AWS infrastructure
- **CI/CD Pipelines**: Setting up automated build and deployment workflows with GitLab CI
- **Cloud Services**: Understanding and implementing various AWS services
- **Container Orchestration**: Deploying and managing containerized microservices with ECS
- **Networking**: Configuring VPC, subnets, security groups, and load balancers
- **Security**: Implementing IAM roles, policies, and secure service communication

## Overview Diagram

![aws-cendence drawio](https://github.com/user-attachments/assets/b7650a30-f5b2-4039-bc37-395013c96d6a)


## Architecture

For this learning project, I built a complete infrastructure for a Transcendence application with:

- Frontend service built with Vite/ThreeJS
- Authentication service using Django
- Game service using Django
- Matchmaking service using Django
- Python AI service
- PostgreSQL database service

All components are containerized and deployed on AWS using:

- **Amazon ECS** with Fargate Spot for cost-effective container orchestration
- **Amazon ECR** for Docker image storage
- **VPC with public and private subnets** for network isolation
- **Application Load Balancer** for traffic distribution
- **AWS Service Discovery** for inter-service communication
- **CloudWatch** for monitoring and logging
- **IAM Roles and Policies** for security
- **VPC Endpoints** for secure access to AWS services

## CI/CD Pipeline

As part of my learning, I implemented a GitLab CI/CD pipeline that automates:

1. Building Docker images for each microservice
2. Running tests to ensure code quality
3. Pushing images to Amazon ECR
4. Deploying updated services to ECS

## Key Challenges and Learnings

During this project, I encountered and overcame several challenges:

- **Service Discovery Configuration**: Understanding how containerized services communicate
- **IAM Permissions**: Learning the principle of least privilege for secure deployments
- **VPC Endpoint Configuration**: Setting up private access to AWS services
- **Pipeline Optimization**: Reducing build times and ensuring reliable deployments
- **Terraform State Management**: Maintaining infrastructure state across multiple deployments

## Project Structure

The project consists of various Terraform configuration files organizing different aspects of the infrastructure:

- Networking configuration (VPC, subnets, security groups)
- ECS cluster and services
- IAM roles and policies
- ECR repositories
- Service discovery namespace
- CloudWatch logging

## Conclusion

This project has been invaluable for my understanding of modern DevOps practices and cloud infrastructure. Through practical implementation, I've gained skills that would be difficult to acquire through theoretical learning alone.

The experience of troubleshooting real-world issues, optimizing configurations, and seeing the entire system working together has provided me with a solid foundation in cloud infrastructure that I can apply to future projects.

## Future Improvements

If I were to continue developing this project, I would explore:

- Implementing auto-scaling based on load metrics
- Adding a CDN for static content delivery
- Setting up disaster recovery and backup procedures
- Implementing blue/green deployment strategies
- Adding comprehensive monitoring and alerting
