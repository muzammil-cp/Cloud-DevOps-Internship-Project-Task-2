# 06 — Amazon S3 Storage Architecture

## Objective
Document the S3 storage component used in Task 2.

## Configuration
- S3 bucket: use the actual bucket name
- Region: same deployment region where appropriate
- Storage class: S3 Standard
- Versioning: enabled
- Public access: blocked unless explicitly required

## Commands

```bash
aws s3 ls
aws s3 ls s3://YOUR_BUCKET_NAME
```

Create a test file:

```bash
echo "Cloud DevOps Internship - AWS S3 Task 2" > s3-test.txt
```

## Verification
Confirm the bucket, versioning status and uploaded object in the AWS Console.

## Image
`06_s3_storage_architecture.png`
