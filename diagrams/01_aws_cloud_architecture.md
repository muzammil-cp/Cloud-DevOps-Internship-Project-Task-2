# 01 — AWS Cloud Architecture

## Objective
Show the complete AWS architecture used for Task 2.

## Components
- AWS Region: `ap-south-1` (replace if another region was used)
- VPC: `cloud-devops-vpc` — `10.0.0.0/16`
- Public subnet: `public-subnet` — `10.0.1.0/24`
- Internet Gateway: `cloud-devops-igw`
- Security Group: `web-server-sg`
- EC2: `cloud-devops-web-server`
- Nginx web server
- IAM, S3 and CloudWatch

## Traffic Flow
Internet → Internet Gateway → Public Subnet → Security Group → EC2/Nginx.

## Verification
Confirm the resource names, CIDRs and services against the actual AWS deployment.

## Image
`01_aws_cloud_architecture.png`
