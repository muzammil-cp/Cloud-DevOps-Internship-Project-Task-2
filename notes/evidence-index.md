# Task 2 Evidence Index

## Project

**Cloud & DevOps Internship — Task 2**

This document maps the Task 2 implementation activities to their corresponding screenshots, documentation, diagrams, and evidence files.

---

## Screenshot Evidence

| No. | Evidence | Screenshot File | Related Documentation |
|---:|---|---|---|
| 01 | Root account MFA | `01_root_account_mfa.png` | `docs/aws-account-security.md` |
| 02 | IAM user | `02_iam_user.png` | `docs/iam-configuration.md` |
| 03 | IAM MFA | `03_iam_mfa.png` | `docs/iam-configuration.md` |
| 04 | VPC created | `04_vpc_created.png` | `docs/vpc-networking.md` |
| 05 | Public subnet | `05_public_subnet.png` | `docs/vpc-networking.md` |
| 06 | Internet Gateway | `06_internet_gateway.png` | `docs/vpc-networking.md` |
| 07 | Public route table | `07_public_route_table.png` | `docs/vpc-networking.md` |
| 08 | Security Group | `08_security_group.png` | `docs/security-groups.md` |
| 09 | EC2 running | `09_ec2_instance_running.png` | `docs/ec2-deployment.md` |
| 10 | EC2 SSH connection | `10_ec2_ssh_connection.png` | `docs/ec2-deployment.md` |
| 11 | Nginx running | `11_nginx_running.png` | `docs/nginx-deployment.md` |
| 12 | Nginx browser page | `12_nginx_browser.png` | `docs/nginx-deployment.md` |
| 13 | Custom Nginx webpage | `13_custom_nginx_webpage.png` | `docs/nginx-deployment.md` |
| 14 | S3 bucket | `14_s3_bucket_created.png` | `docs/s3-storage.md` |
| 15 | S3 versioning | `15_s3_versioning.png` | `docs/s3-storage.md` |
| 16 | S3 object | `16_s3_object_uploaded.png` | `docs/s3-storage.md` |
| 17 | CloudWatch metrics | `17_cloudwatch_ec2_metrics.png` | `docs/cloudwatch-monitoring.md` |
| 18 | CloudWatch alarm | `18_cloudwatch_alarm.png` | `docs/cloudwatch-monitoring.md` |
| 19 | AWS Pricing Calculator | `19_aws_pricing_calculator.png` | `cost/cost-estimation.md` |
| 20 | AWS Billing | `20_aws_billing_cost.png` | `cost/cost-estimation.md` |

> Screenshot filenames should match the actual files in the `screenshots/` directory. Remove or rename entries if a screenshot was not actually captured.

---

# Architecture Diagram Evidence

| No. | Diagram | File | Purpose |
|---:|---|---|---|
| 01 | AWS Cloud Architecture | `diagrams/01_aws_cloud_architecture.png` | Complete infrastructure overview |
| 02 | IAM Security Flow | `diagrams/02_iam_security_flow.png` | IAM and account security |
| 03 | VPC Network Layout | `diagrams/03_vpc_network_layout.png` | VPC and subnet architecture |
| 04 | EC2 Deployment Flow | `diagrams/04_ec2_deployment_flow.png` | EC2 provisioning workflow |
| 05 | Nginx Web Traffic Flow | `diagrams/05_nginx_web_traffic_flow.png` | Web traffic path |
| 06 | S3 Storage Architecture | `diagrams/06_s3_storage_architecture.png` | S3 storage and versioning |
| 07 | CloudWatch Monitoring Flow | `diagrams/07_cloudwatch_monitoring_flow.png` | Monitoring architecture |
| 08 | Security Group Rule Model | `diagrams/08_security_group_rule_model.png` | Security rules |
| 09 | Task 2 Deployment Lifecycle | `diagrams/09_task2_deployment_lifecycle.png` | End-to-end workflow |

---

# Documentation Evidence

| Document | Purpose |
|---|---|
| `docs/aws-account-security.md` | AWS account and MFA security |
| `docs/iam-configuration.md` | IAM configuration |
| `docs/vpc-networking.md` | VPC networking |
| `docs/ec2-deployment.md` | EC2 deployment |
| `docs/nginx-deployment.md` | Nginx configuration |
| `docs/s3-storage.md` | S3 storage configuration |
| `docs/cloudwatch-monitoring.md` | CloudWatch monitoring |
| `docs/security-groups.md` | Security Group configuration |
| `docs/deployment-guide.md` | Complete deployment procedure |

---

# Cost Evidence

| Evidence | File |
|---|---|
| Cost estimation | `cost/cost-estimation.md` |
| Pricing Calculator screenshot | `screenshots/19_aws_pricing_calculator.png` |
| Billing screenshot | `screenshots/20_aws_billing_cost.png` |

---

# Log Evidence

| Log | Purpose |
|---|---|
| `logs/aws-infrastructure.log` | AWS infrastructure configuration record |
| `logs/deployment.log` | EC2/Nginx deployment record |
| `logs/README.md` | Log documentation |

---

# Configuration Evidence

| Configuration | Location |
|---|---|
| AWS region | `config/aws-region.txt` |
| Git/security rules | `.gitignore` |
| Project overview | `README.md` |
| License | `LICENSE` |

---

# Final Submission Evidence

The repository should contain evidence for the following areas:

## 1. Account Security

- Root MFA
- IAM user
- IAM MFA

## 2. Networking

- VPC
- Public subnet
- Internet Gateway
- Route table

## 3. Security

- Security Group
- Restricted SSH
- Protected credentials

## 4. Compute

- EC2 instance
- Ubuntu Server
- SSH connection

## 5. Web Server

- Nginx installation
- Nginx service
- Browser verification
- Custom webpage

## 6. Storage

- S3 bucket
- Versioning
- Test object

## 7. Monitoring

- CloudWatch metrics
- CloudWatch alarm

## 8. Cost

- AWS Pricing Calculator
- Cost estimation document

## 9. Documentation

- Markdown documentation
- Architecture diagrams
- Logs
- Evidence index

---

# Evidence Verification Checklist

- [ ] Screenshot files exist
- [ ] Screenshot names match this index
- [ ] Architecture diagrams exist
- [ ] Documentation files exist
- [ ] Cost estimation exists
- [ ] Logs exist
- [ ] AWS region is documented
- [ ] No private credentials are present
- [ ] No private SSH key is present
- [ ] No AWS secret keys are present
- [ ] README exists
- [ ] LICENSE exists
- [ ] Git status is clean before final submission
