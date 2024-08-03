# k8s-jenkins-cicd-deployment

Overview
This project demonstrates a complete real-time deployment process on a Kubernetes cluster using Jenkins for Continuous Integration and Continuous Deployment (CI/CD). The setup involves multiple EC2 instances, each configured with specific tools to facilitate the deployment pipeline.

Pre-requisites
Before starting, ensure you have the following installed and configured:

1. Git: Version control system for managing code repositories.
2. Linux: Operating system for running the server instances.
3. Jenkins: Automation server for building, deploying, and managing projects.
4. Docker: Platform for containerizing applications.
5. DockerHub Account: For storing and managing Docker images.
6. Ansible: Automation tool for managing configurations and deployments.
7. Kubernetes: Container orchestration platform (specifically focusing on Deployments and Services).
Infrastructure Setup

The project is structured across three EC2 instances, each serving a specific role:

1. Jenkins Instance
Pre-installed with default-jre and Jenkins.
Handles the automation of the build and deployment pipeline.

2. Ansible Instance
Configured with Python, Ansible, and Docker.
Used for configuration management and orchestrating the deployment process across the infrastructure.

3. Web Application Instance (Kubernetes Cluster)
Configured with Docker and Minikube (a tool for running a single-node Kubernetes cluster locally).
Hosts the Kubernetes cluster where the web application will be deployed.

Deployment Process
1. Jenkins will automate the CI/CD pipeline.
2. Ansible will manage the configuration and deployment process.
3. Docker images will be built and pushed to DockerHub.
4. The web application will be deployed on the Kubernetes Cluster using Minikube.

