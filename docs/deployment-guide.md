# Deployment Guide

## Objective

Provide a complete deployment procedure for the AWS Cloud Infrastructure Provisioning Task.

## Requirements

- AWS account
- IAM user
- MFA
- AWS region
- VPC
- Public subnet
- Internet Gateway
- Route table
- Security Group
- EC2 instance
- Nginx
- S3 bucket
- CloudWatch

## Configuration

The deployment consists of the following infrastructure:

```text
Internet
   |
Internet Gateway
   |
VPC 10.0.0.0/16
   |
Public Subnet 10.0.1.0/24
   |
Security Group
   |
Ubuntu EC2
   |
Nginx Web Server
