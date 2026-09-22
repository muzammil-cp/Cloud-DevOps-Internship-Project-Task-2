# Task 2 Requirements & Final Submission Checklist

## Source
Cloud Computing & DevOps Internship — Task 2: Cloud Infrastructure Provisioning with AWS – IAM, VPC, EC2, S3 & Secure Networking.

## Final Submission Checklist

| Internship requirement | Status | Evidence |
|---|---|---|
| AWS Architecture Diagram | Completed | `diagrams/01_aws_cloud_architecture.png` and `screenshots/19.1_aws_architecture_diagram.png` |
| GitHub Repository | Completed | Repository root with README, docs, diagrams, logs, notes and screenshots |
| Infrastructure Report (PDF) | Completed | `docs/AWS_Infrastructure_Report.pdf` |
| IAM Configuration screenshots | Completed | `screenshots/02.1_iam_create_user.png`, `02.2_iam_users.png`, `03.1`–`03.7` |
| VPC screenshots | Completed | `screenshots/04.1`–`07.1` |
| EC2 screenshots | Completed | `screenshots/09.1`, `09.2`, `10.1` |
| Security Group screenshot | Completed | `screenshots/08.1_security_group.png` |
| S3 screenshots | Completed | `screenshots/14.1`, `16.1`, `16.2` |
| CloudWatch Dashboard screenshot | Completed | `screenshots/17.1_cloudwatch_dashboard.png` |
| README.md | Completed | `README.md` |
| Cost Estimation Report | Completed | `cost/cost-estimation.md` |
| Deployment Documentation | Completed | `docs/deployment-guide.md` and service-specific documents |

## Required Infrastructure Evidence

- Root account MFA: documented.
- `DevOpsAdmin`: documented.
- `CloudIntern`: documented.
- `DevOpsAdmins` group and lab `AdministratorAccess`: documented.
- IAM user MFA: documented.
- IAM role `EC2-S3-Access`: documented.
- Custom VPC: `cloud-devops-vpc` (`10.0.0.0/16`).
- Public subnet: `public-subnet` (`10.0.1.0/24`).
- Private subnet: `private-subnet` (`10.0.2.0/24`, `ap-south-1a`, public IPv4 auto-assignment disabled).
- Internet Gateway: `cloud-devops-igw`.
- Public and private route tables: documented.
- Security Group: documented.
- Ubuntu EC2 and SSH: documented.
- Nginx: documented and browser verified.
- S3 versioning and object upload: documented.
- CloudWatch dashboard and CPU alarm: documented.
- AWS Pricing Calculator estimate: documented as USD 15.84/month and USD 190.08/year in the project evidence.

## Advanced Challenge Note

The source document describes static S3 website deployment as an advanced challenge/practice exercise. It is not listed among the final submission checklist items in Section 19, and this repository does not claim that the public static-website challenge was completed unless separate evidence is provided.

## Security Check

Do not commit AWS access keys, secret keys, passwords, MFA secrets, private SSH keys, or other credentials.
