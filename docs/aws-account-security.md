# AWS Account Security

## Objective

Secure the AWS account before performing the Task 2 cloud infrastructure deployment.

## Requirements

- AWS account
- Root account access
- Multi-Factor Authentication (MFA)
- IAM user
- Secure password
- AWS region selected for deployment

## Configuration

The AWS root account was secured using MFA.

An IAM administrative user was created for normal AWS management activities.

The root account is not intended for regular infrastructure administration.

## Commands

AWS account security configuration is primarily performed through the AWS Management Console.

Useful verification command:

```bash
aws sts get-caller-identity
