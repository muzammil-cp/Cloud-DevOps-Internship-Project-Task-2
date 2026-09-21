# 04 — EC2 Deployment Flow

## Objective

Show the EC2 provisioning and verification workflow.

## Flow

```text
VPC
 |
Public Subnet
 |
Security Group
 |
Ubuntu EC2
 |
SSH
 |
Nginx
```

## Configuration

```text
VPC: cloud-devops-vpc
Subnet: public-subnet
Security Group: web-server-sg
Key pair: cloud-devops-key
Instance type: t3.micro
```

## Verification

On the Ubuntu instance:

```bash
hostname
uname -a
ip addr
```

## Image

`04_ec2_deployment_flow.png`
