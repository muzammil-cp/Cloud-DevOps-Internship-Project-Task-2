# 02 — IAM and Account Security

## Objective

Document the account and IAM security model used for Task 2.

## Components

- Root account MFA
- IAM user: `DevOpsAdmin`
- IAM user: `CloudIntern`
- IAM group: `DevOpsAdmins`
- Lab policy: `AdministratorAccess`
- IAM user MFA
- IAM role: `EC2-S3-Access` (trusted entity: EC2)

## Flow

```text
Root MFA
   |
IAM Users
   |
+-- DevOpsAdmin
+-- CloudIntern
   |
DevOpsAdmins Group
   |
AdministratorAccess (lab)
   |
AWS Services
```

## Verification

Use the AWS Console and, if configured, verify the identity with:

```bash
aws sts get-caller-identity
```

## Security Note

Never include passwords, access keys, secret keys, MFA secrets, or private SSH keys in this repository.

## Image

`02_iam_security_flow.png`
