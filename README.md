# AWS Cloud Infrastructure Provisioning

## Cloud & DevOps Internship — Task 2

This project documents the AWS cloud infrastructure provisioned for the **Cloud & DevOps Internship — Task 2**.

The implementation covers identity and access management, VPC networking, EC2 compute, Nginx, S3 storage, CloudWatch monitoring, security controls, architecture documentation, and cost estimation.

---

## Objective

Design, deploy, secure, monitor, and document a basic AWS cloud infrastructure environment using core AWS services.

### Implemented Components

- AWS IAM
- Amazon VPC
- Public and private subnets
- Internet Gateway
- Public and private route tables
- Security Group
- Amazon EC2
- Ubuntu Server
- Nginx Web Server
- Amazon S3
- Amazon CloudWatch
- AWS Pricing Calculator

---

## AWS Region

```text
Region: ap-south-1
Region Name: Asia Pacific (Mumbai)
```

---

## IAM Configuration

The Task 2 IAM setup includes:

- `DevOpsAdmin`
- `CloudIntern`
- `DevOpsAdmins` group
- `AdministratorAccess` through the group for the internship laboratory
- MFA configured for the IAM users
- Root account MFA
- IAM role evidence: `EC2-S3-Access`

The IAM Roles page is documented in `docs/iam-configuration.md` and evidenced by `screenshots/03.3_iam_roles.png`.

---

## Network Configuration

| Resource | Configuration |
|---|---|
| VPC | `cloud-devops-vpc` |
| VPC CIDR | `10.0.0.0/16` |
| Public subnet | `public-subnet` — `10.0.1.0/24` |
| Private subnet | `private-subnet` — `10.0.2.0/24` |
| Availability Zone | `ap-south-1a` |
| Internet Gateway | `cloud-devops-igw` |
| Public route table | `public-route-table` |
| Private route table | `private-route-table` |

The private subnet does not have a direct Internet Gateway route; its route table contains the VPC-local route.

---

## Compute and Web Server

```text
EC2:
  Name: cloud-devops-web-server
  AMI: Ubuntu
  Instance type: t3.micro
  Key pair: cloud-devops-key
  Subnet: public-subnet
  Security Group: web-server-sg

Web Server:
  Nginx
```

---

## S3 Storage

```text
Bucket: muzammil-cloud-devops-task2-2026
Region: ap-south-1
Versioning: Enabled
```

The S3 bucket was used for object storage and the Task 2 test object.

---

## CloudWatch Monitoring

CloudWatch monitoring was configured for the EC2 infrastructure.

A CPU utilization alarm was configured for:

```text
EC2 CPUUtilization > 70%
Alarm: ec2-CPU-High-70
```

---

## Cost Estimation

The AWS Pricing Calculator evidence documents:

```text
Estimated monthly cost: USD 15.84
Estimated 12-month cost: USD 190.08
```

Actual AWS charges can differ depending on usage, data transfer, storage, taxes, pricing changes, and Free Tier eligibility.

---

## Repository Structure

```text
config/       AWS region configuration
cost/         Cost estimation
diagrams/     Architecture and workflow diagrams
docs/         Infrastructure documentation and report
logs/         Project configuration/deployment logs
notes/        Completion and evidence notes
screenshots/  AWS implementation evidence
```

---

## Security

- Root MFA was enabled.
- IAM users were used for laboratory administration.
- MFA was configured for IAM users.
- Permissions were managed through an IAM group.
- SSH access was restricted to the administrator's IP in the documented Security Group configuration.
- AWS credentials, passwords, MFA secrets, and private SSH keys are excluded from the repository.

---

## Deliverables

- AWS Architecture Diagram
- GitHub Repository
- Infrastructure Report PDF
- IAM/VPC/EC2/Security Group/S3/CloudWatch screenshots
- README.md
- Cost Estimation Report
- Deployment Documentation
- Evidence Index

---

## Evidence

See [`notes/evidence-index.md`](notes/evidence-index.md) for the complete mapping between requirements, screenshots, documentation, and diagrams.
