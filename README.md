# PIPEWATCH

<p align="center">

![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-Backend-339933)
![Express](https://img.shields.io/badge/Express.js-API-black)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-D24939)
![n8n](https://img.shields.io/badge/n8n-Automation-FF6D5A)
![Lambda](https://img.shields.io/badge/AWS-Lambda-FF9900)
![EventBridge](https://img.shields.io/badge/EventBridge-Event--Driven-purple)
![DynamoDB](https://img.shields.io/badge/DynamoDB-NoSQL-4053D6)
![API Gateway](https://img.shields.io/badge/API-Gateway-blue)
![License](https://img.shields.io/badge/License-Academic-green)

</p>

---

# Project Overview

**PipeWatch** is a cloud-native DevOps monitoring platform that centralizes **CI/CD pipeline monitoring**, **deployment tracking**, and **AWS infrastructure visibility** into a single real-time dashboard.

Instead of switching between Jenkins, AWS Console, CloudWatch, deployment logs, and multiple monitoring tools, PipeWatch provides a unified interface where DevOps engineers can monitor the complete deployment lifecycle from one place.

The platform combines **AWS Cloud Services**, **Jenkins**, **GitHub**, **Node.js**, **React.js**, and **n8n Automation** to provide real-time monitoring, deployment analytics, and automated notifications.

---

# Problem Statement

Modern DevOps teams often struggle with:

- Monitoring CI/CD pipelines across multiple platforms.
- Tracking deployment history.
- Monitoring AWS infrastructure health.
- Identifying deployment failures quickly.
- Switching between Jenkins, CloudWatch, AWS Console and logs.
- Lack of centralized visibility.

PipeWatch addresses these challenges by providing a single cloud-based monitoring platform.

---

# Features

- Live Jenkins Pipeline Monitoring
- Deployment History Tracking
- AWS Infrastructure Monitoring
- Interactive Dashboard & Charts
- Auto Refresh Dashboard
- Event-Driven Architecture
- Automated Deployment Notifications
- Secure IAM-based Access Control
- CI/CD Automation
- Build Success & Failure Analytics

---

# System Architecture

```
Developer
      │
      ▼
GitHub Repository
      │
      ▼
GitHub Webhook
      │
      ▼
Jenkins (Hosted on EC2)
      │
      ▼
Pipeline Execution
      │
      ├──────────────► Deploy Website to Amazon S3
      │
      ▼
Amazon EventBridge
      │
      ▼
AWS Lambda
      │
      ▼
Amazon DynamoDB
      │
      ▼
Amazon API Gateway
      │
      ▼
Node.js + Express Backend
      │
      ▼
React Dashboard
      │
      ▼
End User
```

---

# AWS Services Used

| Service | Purpose |
|----------|---------|
| IAM | Secure access management |
| EC2 | Hosting Jenkins |
| S3 | Static Website Hosting |
| Lambda | Event Processing |
| EventBridge | Event Routing |
| API Gateway | REST API |
| DynamoDB | Deployment History Storage |
| CloudWatch | Monitoring |
| CloudTrail | Activity Logging |

---

#Technology Stack

## Frontend

- React.js
- Vite
- Recharts
- HTML
- CSS

## Backend

- Node.js
- Express.js

## DevOps

- Jenkins
- GitHub
- n8n
- AWS CLI

## Cloud Platform

- Amazon Web Services (AWS)

---

# CI/CD Workflow

```
Developer Pushes Code
          │
          ▼
GitHub Repository
          │
          ▼
GitHub Webhook
          │
          ▼
Jenkins Pipeline
          │
 ┌────────┼────────┐
 │        │        │
 ▼        ▼        ▼
Checkout Validate Deploy
                  │
                  ▼
             Amazon S3
                  │
                  ▼
           Publish Event
                  │
                  ▼
          Amazon EventBridge
                  │
                  ▼
            AWS Lambda
                  │
                  ▼
           Amazon DynamoDB
                  │
                  ▼
          API Gateway
                  │
                  ▼
      React Monitoring Dashboard
```

---

# Dashboard Modules

The dashboard consists of multiple monitoring sections:

- Dashboard
- Pipeline Monitor
- Deployment History
- Infrastructure Monitoring
- Notifications
- Build Analytics
- Deployment Analytics

---

# Dashboard Metrics

The system visualizes:

- Build Success Rate
- Failure Rate
- Deployment Trend
- Pipeline Duration
- Infrastructure Health
- Jenkins Status
- AWS Resource Status

---

# Security

PipeWatch follows AWS security best practices.

Implemented security features include:

- IAM Users
- Least Privilege Policies
- AWS Access Keys
- Secure REST APIs
- Role-based AWS Access
- Restricted Cloud Permissions

---

# Project Structure

```
PipeWatch/

│
├── frontend/
│     ├── src/
│     ├── components/
│     ├── charts/
│     ├── pages/
│     └── services/
│
├── backend/
│     ├── routes/
│     ├── controllers/
│     ├── services/
│     ├── middleware/
│     └── utils/
│
├── jenkins/
│     └── Jenkinsfile
│
├── infra/
│
├── screenshots/
│
├── demo/
│
└── README.md
```

---

# Key Functionalities

✅ Real-Time Jenkins Monitoring

✅ AWS Infrastructure Monitoring

✅ Automated Deployment Tracking

✅ Event Processing using Lambda

✅ REST APIs

✅ Deployment Analytics

✅ Automated Notifications

✅ Unified DevOps Dashboard

---

# Demo Video

Since this project was developed entirely on AWS Cloud, a complete demonstration video has been included with this repository.

The demo showcases:

- Project Overview
- Complete AWS Architecture
- Jenkins Pipeline Execution
- GitHub Integration
- CI/CD Workflow
- AWS Service Integration
- Live Dashboard
- Deployment Monitoring
- Notification Workflow
- Final Output

 **Please refer to the Demo Video to view the complete working implementation of the project.**
 https://drive.google.com/file/d/1PxiX3IRlv7XKR_xTLVkxjkRzL_O7megi/view?usp=sharing
---

# ⚠ Important Notice

## AWS Infrastructure Status

PipeWatch is a **Cloud & DevOps Project**, and every major component was deployed and executed on AWS Cloud.

During development, the project utilized:

- Amazon EC2
- Jenkins Server
- n8n Server
- Amazon S3
- AWS Lambda
- Amazon EventBridge
- Amazon API Gateway
- Amazon DynamoDB
- IAM
- CloudWatch
- CloudTrail

After the successful completion, testing, and demonstration of the project, **all AWS resources created specifically for PipeWatch were intentionally decommissioned and deleted**.

This includes:

- EC2 Instances
- Jenkins Server
- n8n Server
- Lambda Functions
- API Gateway
- DynamoDB Tables
- EventBridge Resources
- IAM Resources created for the project
- S3 Deployment Bucket
- CloudWatch Resources
- Temporary Testing Resources

This decision was made to:

- Optimize AWS Academy Credits
- Prevent unnecessary cloud costs
- Follow responsible cloud resource management practices

Therefore, the live cloud deployment is no longer available.

---

# Future Enhancements

- Docker Support
- Kubernetes Deployment
- Prometheus Integration
- Grafana Dashboard
- Slack Notifications
- AI Failure Prediction
- Multi Pipeline Support
- Multi Cloud Monitoring
- Role Based Authentication
- Advanced Analytics

---

#  Team

## Team ERROR 420

**Team Leader**

**Athish M**

Register Number: **7376241CS136**

---

**Team Member**

**Vijay Haripriyan D**

Register Number: **7376242AD341**

---

#  Acknowledgement

We sincerely thank our faculty members and mentors for their continuous guidance, encouragement, and support throughout the development of this project.

This project helped us gain practical experience in AWS Cloud Computing, DevOps, CI/CD, Full-Stack Development, and Event-Driven Architecture.

---

# License

This project was developed for **academic and educational purposes**.

© Team ERROR 420
