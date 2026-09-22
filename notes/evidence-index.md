# Task 2 Evidence Index

## Project

**Cloud & DevOps Internship — Task 2**

This document maps the Task 2 implementation activities to screenshots, documentation, diagrams, and evidence files.

---

## Screenshot Evidence

| No. | Evidence | Screenshot File | Related Documentation |
|---:|---|---|---|
| 1 | Root account MFA dashboard | `01.1_root_mfa_dashboard.png` | `docs/aws-account-security.md` |
| 2 | Root account MFA security credentials | `01.2_root_security_credentials_mfa.png` | `docs/aws-account-security.md` |
| 3 | IAM user creation, group and AdministratorAccess | `02.1_iam_create_user.png` | `docs/iam-configuration.md` |
| 4 | IAM users — current final list showing DevOpsAdmin and CloudIntern | `02.2_iam_users.png` | `docs/iam-configuration.md` |
| 5 | IAM user MFA evidence | `03.1_iam_user_mfa.png` | `docs/iam-configuration.md` |
| 6 | CloudIntern MFA assignment | `03.2_cloudintern_mfa.png` | `docs/iam-configuration.md` |
| 7 | IAM Roles | `03.3_iam_roles.png` | `docs/iam-configuration.md` |
| 8 | CloudIntern create-user details | `03.4_cloudintern_create_user_details.png` | `docs/iam-configuration.md` |
| 9 | CloudIntern permissions/group step | `03.5_cloudintern_permissions_group.png` | `docs/iam-configuration.md` |
| 10 | CloudIntern review and create | `03.6_cloudintern_review_and_create.png` | `docs/iam-configuration.md` |
| 11 | CloudIntern created successfully + users list | `03.7_cloudintern_created_successfully_and_users.png` | `docs/iam-configuration.md` |
| 12 | VPC | `04.1_vpc.png` | `docs/vpc-networking.md` |
| 13 | Public subnet | `05.1_public_subnet.png` | `docs/vpc-networking.md` |
| 14 | Private subnet | `05.2_private_subnet.png` | `docs/vpc-networking.md` |
| 15 | Private subnet route table | `05.2_private_subnet_route_table.png` | `docs/vpc-networking.md` |
| 16 | Internet Gateway | `06.1_internet_gateway.png` | `docs/vpc-networking.md` |
| 17 | Public route table | `07.1_route_table.png` | `docs/vpc-networking.md` |
| 18 | Security Group | `08.1_security_group.png` | `docs/security-groups.md` |
| 19 | EC2 launch configuration | `09.1_ec2_launch_configuration.png` | `docs/ec2-deployment.md` |
| 20 | EC2 instance configuration | `09.2_ec2_instance_configuration.png` | `docs/ec2-deployment.md` |
| 21 | SSH connection | `10.1_ssh_connection.png` | `docs/ec2-deployment.md` |
| 22 | Nginx default page | `11.1_nginx_default_page.png` | `docs/nginx-deployment.md` |
| 23 | Nginx browser verification | `12.1_nginx_browser.png` | `docs/nginx-deployment.md` |
| 24 | Custom Nginx webpage | `13.1_custom_nginx_page.png` | `docs/nginx-deployment.md` |
| 25 | S3 bucket and versioning | `14.1_s3_bucket_and_versioning.png` | `docs/s3-storage.md` |
| 26 | S3 object upload | `16.1_s3_object_upload.png` | `docs/s3-storage.md` |
| 27 | S3 uploaded object | `16.2_s3_object_uploaded.png` | `docs/s3-storage.md` |
| 28 | CloudWatch dashboard | `17.1_cloudwatch_dashboard.png` | `docs/cloudwatch-monitoring.md` |
| 29 | CloudWatch alarm configuration | `18.1_cloudwatch_alarm_configuration.png` | `docs/cloudwatch-monitoring.md` |
| 30 | CloudWatch alarm created | `18.2_cloudwatch_alarm_created.png` | `docs/cloudwatch-monitoring.md` |
| 31 | AWS Architecture Diagram | `19.1_aws_architecture_diagram.png` | `diagrams/01_aws_cloud_architecture.md` |
| 32 | AWS Pricing Calculator | `20.1_aws_pricing_calculator.png` | `cost/cost-estimation.md` |

> A separate console-login screenshot for each IAM user is not required by the internship deliverables, so the console-home login screenshot was not added to the evidence set.

---

## IAM Evidence

The IAM implementation includes:

- `DevOpsAdmin`
- `CloudIntern`
- `DevOpsAdmins`
- `AdministratorAccess` through the group for the lab
- MFA evidence for IAM users
- Root account MFA

The CloudIntern creation screenshots explicitly show the username, permissions/review flow, and successful creation. The CloudIntern MFA screenshot confirms that an MFA device was assigned.

**IAM Roles:** `03.3_iam_roles.png` shows the IAM Roles page and the `EC2-S3-Access` role trusted by EC2.

---

## Architecture Diagram Evidence

| No. | Diagram | File | Purpose |
|---:|---|---|---|
| 01 | AWS Cloud Architecture | `diagrams/01_aws_cloud_architecture.png` | Complete AWS infrastructure overview |
| 02 | IAM Security Flow | `diagrams/02_iam_security_flow.png` | IAM and account security |
| 03 | VPC Network Layout | `diagrams/03_vpc_network_layout.png` | VPC, public/private subnets, routes and gateway |
| 04 | EC2 Deployment Flow | `diagrams/04_ec2_deployment_flow.png` | EC2 provisioning and deployment workflow |
| 05 | Nginx Web Traffic Flow | `diagrams/05_nginx_web_traffic_flow.png` | Web traffic path to Nginx |
| 06 | S3 Storage Architecture | `diagrams/06_s3_storage_architecture.png` | S3 storage and versioning |
| 07 | CloudWatch Monitoring Flow | `diagrams/07_cloudwatch_monitoring_flow.png` | CloudWatch monitoring and alerting |
| 08 | Security Group Rule Model | `diagrams/08_security_group_rule_model.png` | Security Group access rules |
| 09 | Task 2 Deployment Lifecycle | `diagrams/09_task2_deployment_lifecycle.png` | End-to-end Task 2 workflow |

---

## Documentation Evidence

| Document | Purpose |
|---|---|
| `docs/aws-account-security.md` | AWS account security and MFA |
| `docs/iam-configuration.md` | IAM users, groups, permissions, MFA, and roles |
| `docs/vpc-networking.md` | VPC, public/private subnets, Internet Gateway, and route tables |
| `docs/ec2-deployment.md` | EC2 deployment and SSH |
| `docs/nginx-deployment.md` | Nginx installation and verification |
| `docs/s3-storage.md` | S3 bucket, object, permissions, and versioning |
| `docs/cloudwatch-monitoring.md` | CloudWatch metrics and alarms |
| `docs/security-groups.md` | Security Group configuration |
| `docs/deployment-guide.md` | Complete deployment procedure |
| `docs/AWS_Infrastructure_Report.pdf` | Final infrastructure report |

---

## Cost Evidence

| Evidence | File |
|---|---|
| Cost estimation | `cost/cost-estimation.md` |
| AWS Pricing Calculator | `screenshots/20.1_aws_pricing_calculator.png` |

Estimated monthly cost documented: **USD 15.84**.

---

## Final Submission Checklist

- [x] Root MFA evidence
- [x] IAM users evidence
- [x] CloudIntern creation workflow evidence
- [x] CloudIntern successful creation evidence
- [x] IAM group evidence/documentation
- [x] IAM user MFA evidence
- [x] IAM Roles page evidence
- [x] Custom VPC
- [x] Public subnet
- [x] Private subnet
- [x] Internet Gateway
- [x] Public route table
- [x] Private route table
- [x] Security Group
- [x] Ubuntu EC2
- [x] SSH evidence
- [x] Nginx evidence
- [x] S3 bucket and versioning
- [x] S3 object evidence
- [x] CloudWatch dashboard
- [x] CloudWatch alarm
- [x] Architecture diagram
- [x] Pricing Calculator evidence
- [x] Cost estimation
- [x] Infrastructure Report PDF
- [x] Logs
- [x] README
- [x] LICENSE
- [x] No AWS access keys or secret keys
- [x] No private SSH keys
- [x] No passwords or MFA secrets
