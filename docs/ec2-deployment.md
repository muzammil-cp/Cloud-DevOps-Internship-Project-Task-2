# EC2 Deployment

## Objective

Deploy an Ubuntu EC2 instance inside the AWS VPC.

## Requirements

- Amazon EC2
- Ubuntu Server AMI
- VPC
- Public subnet
- Security Group
- EC2 key pair

## Configuration

Instance name:

`cloud-devops-web-server`

Operating System:

Ubuntu Server

VPC:

`cloud-devops-vpc`

Subnet:

`public-subnet`

Security Group:

`web-server-sg`

Key Pair:

`cloud-devops-key`

The EC2 instance was configured with a public IPv4 address for remote administration and web access.

## Commands

Connect to the server:

```bash
ssh -i ~/.ssh/cloud-devops-key.pem ubuntu@YOUR_EC2_PUBLIC_IP
