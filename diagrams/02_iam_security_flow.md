# 02 — IAM and Account Security

## Objective
Document the account and IAM security model used for Task 2.

## Components
- Root account MFA
- IAM user: `DevOpsAdmin`
- IAM permissions required for the lab
- IAM user MFA
- AWS services accessed through IAM

## Verification
Use the AWS Console and, if configured, verify the identity with:

```bash
aws sts get-caller-identity
```

## Security Note
Never include passwords, access keys, secret keys, MFA secrets or private SSH keys in this repository.

## Image
`02_iam_security_flow.png`
