# ☁️ AWS Services, DevOps & Cloud Engineering Hands-On Labs

A comprehensive repository documenting my hands-on journey through Cloud Engineering, Infrastructure as Code (IaC), Containerization, CI/CD, and Serverless architectures on Amazon Web Services (AWS). 

This repository serves as a structured archive of real-world deployments, networking lab setups, security configurations, and full-stack cloud hosting patterns developed during my **DevOps and Cloud Engineering Winter & Summer Training programs**.

---

## 🎓 Training & Hands-On Foundation

Through my **Winter and Summer DevOps & Cloud Engineering Training**, I gained deep practical experience in provisioning, securing, and automating cloud infrastructure on AWS. My training focused on moving beyond basic console configurations into architectural best practices, script-based automation, and infrastructure lifecycle management.

### Key Learnings & Practical Exposure:
* **Compute & Web Hosting:** Deploying static, Node.js, and MERN applications on EC2 with Nginx reverse proxies, process management, and custom domain/DNS configurations.
* **Networking & Security:** Building isolated custom VPCs from scratch with public/private subnets, NAT Gateways, Internet Gateways, and strict IAM security policies.
* **Serverless & Event-Driven Systems:** Integrating AWS Lambda, API Gateway, DynamoDB, EventBridge, SNS, and SQS for decoupled, auto-scaling microservices.
* **Infrastructure as Code (IaC) & DevOps Tools:** Provisioning AWS resources via Terraform, writing custom Bash scripts for deployment automation, containerizing apps with Docker, orchestrating with Kubernetes, and setting up CI/CD pipelines using Jenkins and AWS Amplify.

---

## 📂 Repository Structure & Modules

The repository is organized into progressive, hands-on modules covering foundational AWS services up to advanced DevOps pipelines:

```text
AWS_Services/
├── 01_AWS_Infra                         # AWS Cloud Infrastructure Fundamentals
├── 02_AWS_EC2_Server                    # Basic EC2 Instance Setup & Configuration
├── 03_AWS_EC2_Nodejs                    # Node.js Application Hosting on EC2
├── 04_AWS_EC2_Nodejs_Nginx              # Nginx Reverse Proxy & Load Handling for Node.js
├── 05_AWS_EC2_Static_Web                # Static Website Deployment & Vulnerability Patching
├── 06_AWS_EC2_S3                        # Integrating EC2 Applications with S3 Storage
├── 07_AWS_EC2_VPC                       # Custom VPC Setup (Subnets, Route Tables, IGW)
├── 08_AWS_EC2_NAT_Gateway               # Private Subnet Internet Access via NAT Gateway
├── 09_AWS_EC2_MERN_DNS                  # MERN Stack Deployment with Custom DNS Setup
├── 10_AWS_EC2_Nodejs                    # Advanced EC2 Node.js Environment
├── 11_AWS_EC2_Private_Server            # Securing Backend Services in Private Subnets
├── 12_AWS_Revision_Till_Now             # Comprehensive Core AWS Architecture Consolidation
├── 13_AWS_Amplify_Portfolio_Builder     # Full-stack Portfolio Build using AWS Amplify
├── 14_AWS_Baisc_Portfolio               # Cloud-Hosted Personal Portfolio
├── 15_AWS_Lambda_Basics                 # Introduction to Serverless Computing
├── 16_AWS_Lambda_Basics_2/Events        # Event-Driven Trigger Implementations
├── 17_AWS_Amplify                       # AWS Amplify Web Hosting and Backend Services
├── 18_AWS_API_Gateway_Lambda_DynamoDB   # Serverless REST API Architecture (CRUD Operations)
├── 19_AWS_Event_Bridge_SNS_SQS_Lambda   # Asynchronous Event-Driven Messaging Pipeline
├── 20_Linux_Commands                    # Core Linux Administration & Shell Mastery
├── 21_Docker                            # Containerization & Dockerized Node.js CRUD APIs
├── 22_AWS_with_Terraform/EC2            # Infrastructure Provisioning using Terraform
├── 23_Jenkins_Server_in_EC2             # CI/CD Pipeline Automation with Jenkins on EC2
├── 24_Bash_Scripting                    # Shell Scripts for System Administration & Automation
├── 25_Kubernetes                        # Container Orchestration Concepts & Deployments
├── 26_AWS_Amplify_React_App             # Modern React App Deployment on AWS Amplify
└── Reading_Materials                    # Reference Notes & Architectural Diagrams
```

## 🛠️ Tech Stack & Tools Mastered

**Category                                     Technologies & AWS Services**
* **Compute & Web**                            Amazon EC2, Nginx, Node.js, React.js, MERN Stack, AWS Amplify
* **Networking & DNS**                         AWS VPC, Public/Private Subnets, NAT Gateway, Internet Gateway, Route 53
* **Storage & Database**                       Amazon S3, Amazon DynamoDB
* **Serverless & Messaging**                   AWS Lambda, Amazon API Gateway, Amazon EventBridge, Amazon SNS, Amazon SQS
* **DevOps & IaC**                             Terraform, Docker, Kubernetes, Jenkins, Bash / Shell Scripting
* **Security & Admin**                         AWS IAM (Roles, Policies, Trust Relationships), Linux CLI Administration

## 🏗️ Core Architectural Patterns Implemented

### 1. Multi-Tier Secure VPC Architecture (07_AWS_EC2_VPC – 09_AWS_EC2_MERN_DNS)
* Isolated public and private subnets across Availability Zones.
* Configured NAT Gateways to grant private database instances secure outbound internet access for updates while blocking incoming public exposure.

### 2. Serverless Microservices Pipeline (18_AWS_API_Gateway_Lambda_DynamoDB & 19_AWS_Event_Bridge_SNS_SQS_Lambda)
* Exposed REST APIs via API Gateway triggering AWS Lambda functions to write data to DynamoDB.
* Built asynchronous messaging pipelines using EventBridge, SNS, and SQS queues for decoupling application services.

### 3. Automated Deployment & Infrastructure as Code (21_Docker – 23_Jenkins_Server_in_EC2)
* Containerized Node.js applications with Docker.
* Automated EC2 server provisioning using Terraform.
* Deployed a dedicated Jenkins build server on EC2 to automate deployment workflows.

## 🚀 Prerequisites & Getting Started 

### Local Setup Requirements  
* AWS CLI v2 configured with appropriate permissions (aws configure)
* Terraform (>= v1.0)
* Docker Desktop 
* Node.js (v18+) & Git
    
### Clone & Explore
    
      # Clone the repository
      git clone [https://github.com/AdeshYadav8918/AWS_Services.git](https://github.com/AdeshYadav8918/AWS_Services.git)
   
      # Navigate into a specific module (e.g., Serverless REST API)
      cd AWS_Services/18_AWS_API_Gateway_Lambda_DynamoDB_IAM

      # Follow module-specific instructions or inspect script configurations

## 🛡️ Security Best Practices
* Credential Hygiene: All API keys, AWS credentials, and .pem SSH keys are strictly scrubbed and kept out of version control (.gitignore enforced).
* Least Privilege: Infrastructure resources utilize granular IAM roles and scoped policies.
