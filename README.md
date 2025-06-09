# 3-tier-architecture-in-AWS

![image](https://github.com/user-attachments/assets/1fb8c77b-a4bd-4c6d-af54-be14038c884b)

# AWS 3-Tier Architecture (Manual Setup) – DevOps Project

This project demonstrates how I deployed a traditional 3-tier architecture on AWS using manual provisioning and DevOps practices.

## 🧱 Architecture Overview

- **Web Tier:** EC2 instance with Apache/Nginx
- **App Tier:** EC2 instance with a backend application (e.g., Node.js, Python, etc.)
- **DB Tier:** AWS RDS (MySQL/PostgreSQL)

## ⚙️ Tools Used

- **AWS Services:** EC2, RDS, VPC, Security Groups, Elastic Load Balancer
- **Provisioning:** AWS Console (manual setup)
- **Automation:** Bash scripts (user-data), SSH provisioning

In summary:

1. Created custom VPC with public/private subnets
2. Launched EC2 instances for Web and App tier
3. Configured Security Groups to restrict access between layers
4. Launched RDS in a private subnet
5. Used user-data scripts to install and configure software

## 🔐 Security Measures

- Web tier in public subnet with HTTP access
- App and DB tier in private subnet with only internal access
- IAM roles for EC2, where applicable

## 🧠 What I Learned

- VPC/Subnet design and segregation of duties
- Setting up a secure and scalable architecture manually
- Importance of configuration management and documentation

## 📝 Notes

This project can be enhanced further by adding:
- Infrastructure as Code (e.g., Terraform or CloudFormation)
- CI/CD pipeline (GitHub Actions, Jenkins, etc.)
- Monitoring and alerting (CloudWatch, Prometheus)
