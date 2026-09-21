# 01 — AWS Cloud Architecture

## Objective

Show the complete AWS architecture used for Task 2.

## Components

- Region: `ap-south-1` (Asia Pacific — Mumbai)
- VPC: `cloud-devops-vpc` — `10.0.0.0/16`
- Public subnet: `public-subnet` — `10.0.1.0/24`
- Private subnet: `private-subnet` — `10.0.2.0/24`
- Internet Gateway: `cloud-devops-igw`
- Public route table: `public-route-table`
- Private route table: `private-route-table`
- Security Group: `web-server-sg`
- EC2: `cloud-devops-web-server`
- Nginx web server
- IAM: `DevOpsAdmin`, `CloudIntern`, `DevOpsAdmins`
- S3: `muzammil-cloud-devops-task2-2026`
- CloudWatch monitoring and alarm

## Traffic Flow

```text
Internet → Internet Gateway → Public Subnet → Security Group → EC2/Nginx
```

The private subnet is isolated from a direct Internet Gateway route.

## Image

`01_aws_cloud_architecture.png`
