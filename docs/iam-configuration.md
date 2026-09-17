# IAM Configuration

## Objective

Create and configure an IAM user for secure AWS resource administration.

## Requirements

- AWS Management Console
- IAM service
- Administrative IAM permissions for the lab
- MFA

## Configuration

IAM user:

`DevOpsAdmin`

The user was configured with appropriate permissions required to complete the Task 2 laboratory activities.

MFA was enabled to provide an additional authentication factor.

## Commands

Verify the current AWS identity:

```bash
aws sts get-caller-identity
