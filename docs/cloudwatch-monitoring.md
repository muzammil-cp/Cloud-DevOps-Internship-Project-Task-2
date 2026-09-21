# CloudWatch Monitoring

## Objective

Monitor the EC2 infrastructure using Amazon CloudWatch.

## Configuration

The EC2 instance was monitored using CloudWatch.

Reviewed monitoring information:

- CPU utilization
- EC2 instance metrics
- Instance health
- Alarm configuration

## Alarm

```text
Name: ec2-CPU-High-70
Condition: EC2 CPU utilization > 70%
```

## Verification

The CloudWatch dashboard and alarm configuration were verified in the AWS Console.

Useful AWS CLI command:

```bash
aws ec2 describe-instances
```

## Evidence

- `screenshots/17.1_cloudwatch_dashboard.png`
- `screenshots/18.1_cloudwatch_alarm_configuration.png`
- `screenshots/18.2_cloudwatch_alarm_created.png`
