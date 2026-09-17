# CloudWatch Monitoring

## Objective

Monitor the EC2 infrastructure using Amazon CloudWatch.

## Requirements

- Running EC2 instance
- Amazon CloudWatch
- EC2 monitoring
- CloudWatch alarm

## Configuration

The EC2 instance was monitored using CloudWatch.

The following monitoring information was reviewed:

- CPU utilization
- Instance health
- EC2 monitoring metrics

A CloudWatch alarm was configured for the selected EC2 metric.

## Commands

Check EC2 instance information:

```bash
aws ec2 describe-instances
