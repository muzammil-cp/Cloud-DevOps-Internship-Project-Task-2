# AWS Cloud Infrastructure Provisioning

## Cloud & DevOps Internship — Task 2

This project demonstrates the provisioning and configuration of AWS cloud infrastructure using core AWS services.

---

## Objective

The objective of this project is to design, deploy, secure, and document a basic AWS cloud infrastructure environment.

The project includes:

- AWS IAM
- Amazon VPC
- Public Subnet
- Internet Gateway
- Route Table
- Security Group
- Amazon EC2
- Ubuntu Server
- Nginx Web Server
- Amazon S3
- Amazon CloudWatch
- AWS Pricing Calculator

---

## AWS Services Used

| Service | Purpose |
|---|---|
| IAM | Identity and access management |
| VPC | Network isolation |
| Subnet | Network segmentation |
| Internet Gateway | Internet connectivity |
| Route Table | Network routing |
| Security Group | Instance-level network security |
| EC2 | Cloud compute server |
| Nginx | Web server |
| S3 | Object storage |
| CloudWatch | Monitoring and alarms |
| Pricing Calculator | Cost estimation |

---

## Architecture

The infrastructure follows this basic architecture:

```text
                         Internet
                            |
                            |
                   Internet Gateway
                            |
                +-----------+-----------+
                |                       |
                |        AWS VPC        |
                |      10.0.0.0/16      |
                |                       |
                |   Public Subnet       |
                |    10.0.1.0/24        |
                |          |            |
                |          |            |
                |    Security Group     |
                |          |            |
                |          |            |
                |    Ubuntu EC2         |
                |    Nginx Web Server   |
                |                       |
                +-----------------------+

          IAM              S3              CloudWatch
           |                |                   |
           +----------------+-------------------+
                            |
                       AWS Services
