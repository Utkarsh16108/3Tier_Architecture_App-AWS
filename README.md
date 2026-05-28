# Welcome  👋

**AWS 3-Tier Architecture Application Deployment with High Availability & Fault Tolerance**

**Project Overview**
This project demonstrates the deployment of a highly available and fault-tolerant 3-Tier Web Application Architecture on AWS. The infrastructure is designed following cloud best practices by separating the application into Web Tier, Application Tier, and Database Tier to ensure scalability, security, maintainability, and high availability.

The project leverages AWS services such as VPC, EC2, RDS, S3, IAM, Application Load Balancer (ALB), SSL/TLS, and Domain Mapping to create a production-like environment.

The architecture ensures secure communication between tiers, internal traffic routing, and efficient load balancing to improve reliability and performance.
<img width="1280" height="582" alt="image" src="https://github.com/user-attachments/assets/bb21cdac-c308-4072-80d0-1363d93c7b56" />



## 🚀 **In this Project, I have used the following AWS services:**

- **VPC**  
- **S3**  
- **IAM**  
- **EC2**  
- **RDS**  
- **Route 53**


**Architecture Overview**

**1. Web Tier**
1. Hosted on EC2 instances in public subnets
2. Configured with Nginx to serve frontend traffic
3. Integrated with an External Application Load Balancer
4. Handles incoming user requests securely using HTTPS (SSL Certificate)

**2. Application Tier**
1. Hosted on EC2 instances in private subnets
2. Node.js-based backend application managed using PM2
3. Internal communication enabled through an Internal Load Balancer
4. Securely communicates with the database layer

**3. Database Tier**
1. Configured using Amazon RDS (MySQL)
2. Deployed in private networking for enhanced security
3. Stores transactional application data
4. Access restricted through Security Groups

**Deployment Workflow**
1. Created a secure VPC Architecture with public and private subnets.
2. Configured S3 Bucket for application storage and IAM role-based access.
3. Launched and configured Amazon RDS MySQL Database.
4. Deployed backend services in the Application Tier using Node.js and PM2.
5.Configured an Internal Load Balancer for secure backend communication.
6. Deployed frontend services in the Web Tier using Nginx.
7. Configured an External Load Balancer for user traffic routing.
8. Enabled SSL/TLS encryption and domain mapping for secure access.

**Tech Stack**

**1. Cloud:** AWS (EC2, VPC, RDS, IAM, S3, ALB)**
**2. Backend:** Node.js
**3. Database:** MySQL (Amazon RDS)
**4. Web Server:** Nginx
**5. Process Manager:** PM2
**6. OS:** Amazon Linux

**Key Features**
1. High Availability Architecture.
2. Fault Tolerant Infrastructure.
3. Internal & External Load Balancing.
4. Secure Private/Public Subnet Segmentation. 
5. SSL-Based Secure Communication. 
6. Scalable Multi-Tier Deployment. 
7. Production-Like AWS Infrastructure.

**Security Implementation**
1. Database deployed in private subnet
2. IAM Role-based access instead of hardcoded credentials
3. Security Group-based communication between tiers
4. HTTPS enabled using SSL/TLS certificates.


