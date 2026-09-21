# S3 Storage

## Objective

Create and configure an Amazon S3 bucket for cloud object storage.

## Configuration

```text
Bucket: muzammil-cloud-devops-task2-2026
Region: ap-south-1
Storage Class: S3 Standard
Versioning: Enabled
```

The bucket was configured with versioning enabled.

Public access was not required for the Task 2 storage evidence.

## Test Object

The test object was created using:

```bash
echo "Cloud DevOps Internship - AWS S3 Task 2" > s3-test.txt
```

The object was uploaded to the S3 bucket and verified in the AWS Console.

## Evidence

- `screenshots/14.1_s3_bucket_and_versioning.png`
- `screenshots/16.1_s3_object_upload.png`
- `screenshots/16.2_s3_object_uploaded.png`

## Security

Do not make an S3 bucket public unless the exercise specifically requires it. Do not store credentials or private keys in S3 or GitHub.
