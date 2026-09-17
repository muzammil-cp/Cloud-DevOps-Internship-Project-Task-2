# S3 Storage

## Objective

Create and configure an Amazon S3 bucket for cloud object storage.

## Requirements

- Amazon S3
- Globally unique bucket name
- AWS region
- Test object

## Configuration

Bucket name:

`[ENTER YOUR ACTUAL BUCKET NAME]`

Region:

`ap-south-1`

Storage Class:

S3 Standard

Versioning:

Enabled

Public access:

Blocked unless explicitly required by the exercise.

## Commands

Create a test file:

```bash
echo "Cloud DevOps Internship - AWS S3 Task 2" > s3-test.txt
