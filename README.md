# 🚀 Highly Available Web Application on AWS

A production-style AWS project demonstrating a **Highly Available Web Application** using **Amazon EC2**, **Application Load Balancer (ALB)**, **Amazon EFS**, and **Auto Scaling Group (ASG)**.

---

## 📌 Project Overview

This project deploys a scalable and highly available web application on AWS.

The application is hosted on multiple EC2 instances behind an Application Load Balancer while sharing website files through Amazon Elastic File System (EFS). Auto Scaling automatically launches or terminates EC2 instances based on demand.

---

## 🏗️ AWS Architecture

```
                    Internet
                        │
                        ▼
        ┌──────────────────────────┐
        │ Application Load Balancer│
        └────────────┬─────────────┘
                     │
          ┌──────────┴──────────┐
          ▼                     ▼
    EC2 Instance 1        EC2 Instance 2
          │                     │
          └──────────┬──────────┘
                     ▼
              Amazon Elastic
               File System
                  (EFS)
```

---

## 🚀 AWS Services Used

- Amazon EC2
- Application Load Balancer (ALB)
- Auto Scaling Group (ASG)
- Amazon Elastic File System (EFS)
- Launch Template
- Target Group
- Security Groups
- Ubuntu Server
- Apache2 Web Server

---

## ⚙️ Features

- Highly Available Architecture
- Automatic Load Distribution
- Shared Storage using Amazon EFS
- Auto Scaling Support
- Launch Template Automation
- Apache Web Server
- Persistent Shared Website Files
- Fault Tolerant Design

---

## 📂 Project Workflow

1. Launch Ubuntu EC2 instances.
2. Install Apache2 automatically using User Data.
3. Install NFS utilities.
4. Mount Amazon EFS.
5. Configure Apache to serve files from EFS.
6. Create a Launch Template.
7. Create an Auto Scaling Group.
8. Register instances with a Target Group.
9. Configure the Application Load Balancer.
10. Access the application using the ALB DNS Name.

---

## 🔧 User Data Script

The Launch Template automatically performs:

- System Update
- Apache Installation
- NFS Installation
- Amazon EFS Mount
- Apache Configuration
- Automatic Startup

---

## 📁 Project Structure

```
Project
│
├── README.md
├── architecture.png
├── userdata.sh
├── screenshots
│   ├── ec2.png
│   ├── efs.png
│   ├── alb.png
│   ├── asg.png
│   ├── target-group.png
│   └── webpage.png
```

---

## 📸 Screenshots

### AWS Architecture

> Add your architecture diagram here.

```
screenshots/architecture.png
```

---

### EC2 Instances

```
screenshots/ec2.png
```

---

### Amazon EFS

```
screenshots/efs.png
```

---

### Application Load Balancer

```
screenshots/alb.png
```

---

### Auto Scaling Group

```
screenshots/asg.png
```

---

### Target Group

```
screenshots/target-group.png
```

---

### Web Application

```
screenshots/webpage.png
```

---

## 🧪 Validation Performed

- Verified Apache Installation
- Verified EFS Mount
- Confirmed Shared Storage Between EC2 Instances
- Verified ALB Health Checks
- Tested Load Balancing
- Tested Auto Scaling Instance Creation
- Confirmed Automatic EFS Mount on New Instances

---

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

- Amazon EC2
- Apache Web Server
- Linux Administration
- SSH & Key Pair Authentication
- Amazon EFS
- NFS Mounting
- Application Load Balancer
- Target Groups
- Auto Scaling Groups
- Launch Templates
- High Availability Architecture
- AWS Networking
- Security Groups
- Infrastructure Automation

---

## 🚀 Future Improvements

- HTTPS using AWS Certificate Manager (ACM)
- Route 53 Domain Integration
- CloudWatch Monitoring
- AWS WAF Integration
- AWS CodePipeline CI/CD
- Terraform Infrastructure as Code
- Docker Container Deployment
- ECS or EKS Migration

---

## 👨‍💻 Author

**Vishnu R**

Cloud & DevOps Enthusiast

GitHub: https://github.com/your-username

LinkedIn: https://linkedin.com/in/your-profile

---

## ⭐ If you found this project helpful, consider giving it a star!
