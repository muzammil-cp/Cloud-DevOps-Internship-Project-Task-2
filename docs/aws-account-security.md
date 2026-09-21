# AWS Account Security

## Objective

Secure the AWS account before performing the Task 2 cloud infrastructure deployment.

## Configuration

The account security implementation includes:

- Root account MFA
- IAM users for laboratory administration
- IAM group-based permissions
- MFA for IAM users
- No AWS credentials stored in the repository

### IAM Users

```text
DevOpsAdmin
CloudIntern
```

### IAM Group

```text
DevOpsAdmins
```

The internship laboratory group uses `AdministratorAccess` as specified by the task instructions.

## Verification

AWS account security configuration is primarily performed through the AWS Management Console.

Useful identity verification command:

```bash
aws sts get-caller-identity
```

## Evidence

- Root MFA dashboard
- Root MFA security credentials
- IAM users
- CloudIntern MFA assignment

Do not store passwords, access keys, secret keys, MFA secrets, or private SSH keys in the repository.
