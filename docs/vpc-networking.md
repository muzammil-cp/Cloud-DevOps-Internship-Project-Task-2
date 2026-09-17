# VPC Networking

## Objective

Create a secure AWS VPC network for the Task 2 infrastructure.

## Requirements

- Amazon VPC
- VPC CIDR block
- Public subnet
- Internet Gateway
- Route table

## Configuration

### VPC

Name:

`cloud-devops-vpc`

CIDR:

`10.0.0.0/16`

### Public Subnet

Name:

`public-subnet`

CIDR:

`10.0.1.0/24`

### Internet Gateway

Name:

`cloud-devops-igw`

The Internet Gateway was attached to the VPC.

### Route Table

Name:

`public-route-table`

Internet route:

```text
0.0.0.0/0
