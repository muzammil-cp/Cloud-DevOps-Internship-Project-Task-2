# Deployment Guide

## Objective

Provide a concise record of the AWS Cloud Infrastructure Provisioning Task 2 deployment.

## Region

```text
ap-south-1 — Asia Pacific (Mumbai)
```

## Deployment Components

1. Secure the AWS account with root MFA.
2. Create IAM users and group-based permissions.
3. Configure IAM user MFA.
4. Create the custom VPC.
5. Create public and private subnets.
6. Attach the Internet Gateway.
7. Configure public and private route tables.
8. Configure the Security Group.
9. Launch the Ubuntu EC2 instance.
10. Connect to the instance using SSH.
11. Install and verify Nginx.
12. Create the S3 bucket and enable versioning.
13. Upload and verify the test object.
14. Configure CloudWatch monitoring and an EC2 CPU alarm.
15. Document the architecture and estimate costs.

## Network

```text
Internet
   |
Internet Gateway
   |
VPC 10.0.0.0/16
   |
   +-- Public Subnet 10.0.1.0/24
   |      |
   |      +-- Security Group
   |      |
   |      +-- Ubuntu EC2 + Nginx
   |
   +-- Private Subnet 10.0.2.0/24
          |
          +-- private-route-table
```

## S3

```text
Bucket: muzammil-cloud-devops-task2-2026
Versioning: Enabled
```

## Monitoring

```text
CloudWatch
    |
    +-- EC2 CPUUtilization
    |
    +-- Alarm: ec2-CPU-High-70
```

## Verification

Use the AWS Console and appropriate AWS CLI commands to verify resources. Never commit credentials or private keys.
