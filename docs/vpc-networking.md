# VPC Networking

## Objective

Create and document the custom AWS VPC network used by the Task 2 infrastructure.

## VPC

```text
Name: cloud-devops-vpc
CIDR: 10.0.0.0/16
Region: ap-south-1
```

## Public Subnet

```text
Name: public-subnet
CIDR: 10.0.1.0/24
Availability Zone: ap-south-1a
```

The public subnet is used by the Ubuntu EC2 web server and is connected to the Internet Gateway through the public route table.

## Private Subnet

```text
Name: private-subnet
CIDR: 10.0.2.0/24
Availability Zone: ap-south-1a
Auto-assign public IPv4: No
```

The private subnet is associated with:

```text
private-route-table
```

## Internet Gateway

```text
Name: cloud-devops-igw
```

The Internet Gateway is attached to `cloud-devops-vpc`.

## Public Route Table

```text
Name: public-route-table
```

The public route table contains the Internet route:

```text
0.0.0.0/0 → Internet Gateway
```

and is associated with the public subnet.

## Private Route Table

```text
Name: private-route-table
```

The private route table is associated with `private-subnet`.

The verified private-subnet design does not contain a direct Internet Gateway route; the VPC-local route remains available for internal communication.

## Evidence

- `04.1_vpc.png`
- `05.1_public_subnet.png`
- `05.2_private_subnet.png`
- `05.2_private_subnet_route_table.png`
- `06.1_internet_gateway.png`
- `07.1_route_table.png`

## Security

The private subnet does not receive a public IPv4 address automatically and is not directly routed to the Internet Gateway.
