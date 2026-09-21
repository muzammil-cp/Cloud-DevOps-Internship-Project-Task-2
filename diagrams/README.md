# Task 2 — Diagrams

This folder contains the architecture and workflow diagrams used to document the AWS Cloud Infrastructure Provisioning project.

## Diagram Set

| No. | Diagram | Purpose |
|---:|---|---|
| 01 | AWS Cloud Architecture | Complete infrastructure overview |
| 02 | IAM and Account Security | IAM users, group, MFA and security flow |
| 03 | VPC Network Layout | VPC, public/private subnets, routes and gateway |
| 04 | EC2 Deployment Flow | EC2 provisioning workflow |
| 05 | Nginx Web Traffic Flow | Internet-to-Nginx traffic |
| 06 | S3 Storage Architecture | S3 object storage and versioning |
| 07 | CloudWatch Monitoring Flow | EC2 monitoring and alarms |
| 08 | Security Group Rule Model | Network access rules |
| 09 | Task 2 Deployment Lifecycle | End-to-end project workflow |

## Important

The diagrams in this repository reflect the documented Task 2 resource configuration:

- Region: `ap-south-1`
- VPC: `cloud-devops-vpc`
- Public subnet: `10.0.1.0/24`
- Private subnet: `10.0.2.0/24`
- S3 versioning: enabled
- CloudWatch CPU alarm: configured

Never include AWS passwords, access keys, secret keys, MFA secrets, private SSH keys, or other credentials.
