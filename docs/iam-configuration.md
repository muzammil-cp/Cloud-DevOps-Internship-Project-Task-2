# IAM Configuration

## Objective

Configure IAM users, groups, permissions, MFA, and roles for secure AWS resource administration during the Task 2 laboratory.

## Internship Requirements

The Task 2 guide requires:

- IAM users
- IAM groups
- Least-privilege awareness
- MFA
- IAM roles
- Policies

For the laboratory instructions, the named users are `DevOpsAdmin` and `CloudIntern`, with `AdministratorAccess` assigned through the lab group.

## IAM Users

Configured users:

- `DevOpsAdmin`
- `CloudIntern`

Both users are associated with:

```text
DevOpsAdmins
```

## IAM Group

```text
Group: DevOpsAdmins
Lab policy: AdministratorAccess
```

The policy is attached through the group rather than separately to each user.

## MFA

MFA evidence is included for the privileged IAM users.

Evidence:

- `screenshots/03.1_iam_user_mfa.png` — IAM user MFA evidence
- `screenshots/03.2_cloudintern_mfa.png` — CloudIntern MFA device assignment
- `screenshots/01.1_root_mfa_dashboard.png` — root account MFA
- `screenshots/01.2_root_security_credentials_mfa.png` — root MFA security credentials

The CloudIntern evidence confirms that an MFA device was successfully assigned.

## IAM Roles

IAM role evidence is included in:

```text
screenshots/03.3_iam_roles.png
```

The AWS IAM Roles page shows four roles, including:

```text
EC2-S3-Access
Trusted entity: AWS Service: ec2
```

This role is relevant to the EC2-to-AWS-service access used in the Task 2 environment.

## Security Practices

- Root account is not intended for routine infrastructure administration.
- IAM users are used for laboratory activities.
- MFA is enabled for privileged access.
- Permissions are managed through an IAM group.
- AWS credentials and secrets are not stored in GitHub.
- Private SSH keys are excluded from version control.

## Verification

```bash
aws sts get-caller-identity
```

Never commit AWS access keys, secret keys, passwords, MFA secrets, or private SSH keys.
