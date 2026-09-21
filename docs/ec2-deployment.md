# EC2 Deployment

## Objective

Deploy and verify an Ubuntu EC2 instance inside the Task 2 VPC.

## Configuration

```text
Instance name: cloud-devops-web-server
Operating system: Ubuntu Server 26.04
Instance type: t3.micro
VPC: cloud-devops-vpc
Subnet: public-subnet
Security Group: web-server-sg
Key pair: cloud-devops-key
```

The launch configuration screenshot shows the instance using the public subnet and `web-server-sg`.

## SSH

The instance was accessed using SSH. Use the private key file that corresponds to the `cloud-devops-key` key pair; do not commit that private key to GitHub.

Example:

```bash
Use the `cloud-devops-key` private key with the EC2 instance's current public IPv4 address.
```

## Verification

Useful commands on the Ubuntu server:

```bash
hostname
uname -a
ip addr
```

## Evidence

- `screenshots/09.1_ec2_launch_configuration.png`
- `screenshots/09.2_ec2_instance_configuration.png`
- `screenshots/10.1_ssh_connection.png`
