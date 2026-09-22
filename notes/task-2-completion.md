# Task 2 Completion Notes

## Project

**Cloud & DevOps Internship — Task 2**

### Title

**AWS Cloud Infrastructure Provisioning with AWS – IAM, VPC, EC2, S3 & Secure Networking**

---

## Objective

Provision, configure, secure, monitor, and document a basic AWS cloud infrastructure environment using AWS core services.

---

## AWS Services Implemented

- AWS IAM
- Amazon VPC
- Public and private subnets
- Internet Gateway
- Route Tables
- Security Group
- Amazon EC2
- Ubuntu Server
- Nginx Web Server
- Amazon S3
- Amazon CloudWatch
- AWS Pricing Calculator

---

## Account Security

- Root account MFA
- `DevOpsAdmin` IAM user
- `CloudIntern` IAM user
- `DevOpsAdmins` IAM group
- `AdministratorAccess` through the lab group
- MFA configured for IAM users
- No credentials or private keys stored in GitHub

---

## IAM

```text
Users:
  DevOpsAdmin
  CloudIntern

Group:
  DevOpsAdmins

Lab policy:
  AdministratorAccess

MFA:
  Root account: enabled
  IAM users: configured
```

The latest CloudIntern evidence confirms an MFA device was assigned. Additional screenshots document the CloudIntern create-user details, permissions/review flow, and successful creation with both IAM users visible.

IAM role evidence is included in `screenshots/03.3_iam_roles.png`. The IAM Roles page shows `EC2-S3-Access` with EC2 as the trusted service.

---

## VPC

```text
VPC: cloud-devops-vpc
CIDR: 10.0.0.0/16

Public subnet:
  public-subnet
  10.0.1.0/24

Private subnet:
  private-subnet
  10.0.2.0/24
  ap-south-1a
  Auto-assign public IPv4: No

Internet Gateway:
  cloud-devops-igw

Public route table:
  public-route-table

Private route table:
  private-route-table
```

---

## EC2 and Nginx

```text
Instance: cloud-devops-web-server
OS: Ubuntu
Instance type: t3.micro
Key pair: cloud-devops-key
Security Group: web-server-sg
Web server: Nginx
```

SSH and Nginx browser verification were captured in the screenshot evidence.

---

## S3

```text
Bucket: muzammil-cloud-devops-task2-2026
Region: ap-south-1
Versioning: Enabled
```

The Task 2 test object was uploaded and verified.

---

## CloudWatch

```text
Alarm: ec2-CPU-High-70
Metric: EC2 CPUUtilization
Threshold: > 70%
```

---

## Cost Estimation

```text
Estimated monthly cost: USD 15.84
Estimated 12-month cost: USD 190.08
```

The estimate is based on the AWS Pricing Calculator screenshot included in the repository. Actual charges can vary.

---

## Documentation

The repository contains:

- README
- IAM documentation
- VPC/networking documentation
- EC2 deployment documentation
- Nginx documentation
- S3 documentation
- CloudWatch documentation
- Security Group documentation
- Deployment guide
- Architecture diagrams
- Logs
- Evidence index
- Infrastructure Report PDF
- Cost estimation report

---

## Security Reminder

Never commit:

- AWS access keys
- AWS secret keys
- Passwords
- MFA secrets
- Private SSH keys
- `.env` files containing credentials
