# 03 — VPC Network Layout

## Objective
Show the VPC networking resources required by Task 2.

## Configuration
- VPC: `10.0.0.0/16`
- Public subnet: `10.0.1.0/24`
- Internet Gateway: `cloud-devops-igw`
- Route: `0.0.0.0/0` to the Internet Gateway
- Public subnet associated with the public route table

## Verification Commands

```bash
aws ec2 describe-vpcs
aws ec2 describe-subnets
aws ec2 describe-route-tables
aws ec2 describe-internet-gateways
```

## Image
`03_vpc_network_layout.png`
