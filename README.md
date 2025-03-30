# Real Estate App - Infrastructure (Terraform)

## Overview
This repository contains the Terraform code for deploying the Real Estate App infrastructure on AWS. The infrastructure includes compute instances, networking, storage, and IAM roles, ensuring a secure and scalable deployment.

## Architecture Diagram
![Architecture](https://raw.githubusercontent.com/y7ksh-r/Real-estate-app-infra/main/docs/architecture.png)  
*Infrastructure: AWS EC2 (for hosting), S3 (for storage), IAM (for access control), and Terraform for provisioning.*

## Features
- **State Locking with S3 & DynamoDB**: Prevents race conditions in Terraform deployments.
- **Infrastructure as Code (IaC)**: Enables reproducible and version-controlled deployments.
- **Secure Access Control**: IAM roles and security groups restrict access.
- **Scalability & Modularity**: Easily extendable to accommodate future changes.

## Real-World Use Case
This Terraform setup allows teams to **quickly provision and manage cloud infrastructure** without manual intervention. It's especially useful for **DevOps workflows** where infrastructure needs to be **version-controlled, auditable, and automated.**

## Deployment Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/y7ksh-r/Real-estate-app-infra.git
   cd Real-estate-app-infra
   ```
2. Initialize Terraform:
   ```sh
   terraform init
   ```
3. Plan the deployment:
   ```sh
   terraform plan
   ```
4. Apply changes:
   ```sh
   terraform apply -auto-approve
   ```
5. Destroy infrastructure (if needed):
   ```sh
   terraform destroy -auto-approve
   ```

## Future Enhancements
- Implement **Terraform modules** for better reusability.
- Integrate **AWS Lambda for automated scaling.**
- Add **monitoring with Prometheus & Grafana.**
