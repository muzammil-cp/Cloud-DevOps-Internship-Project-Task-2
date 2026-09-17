# 04 — EC2 Deployment Flow

## Objective
Show the sequence used to deploy the Ubuntu EC2 web server.

## Steps
1. Select Ubuntu Server AMI.
2. Select the appropriate instance type.
3. Select `cloud-devops-vpc` and `public-subnet`.
4. Attach `web-server-sg`.
5. Select `cloud-devops-key`.
6. Launch the instance.
7. Connect using SSH.
8. Install and configure Nginx.

## Verification

```bash
ssh -i ~/.ssh/cloud-devops-key.pem ubuntu@YOUR_EC2_PUBLIC_IP
hostname
uname -a
ip addr
```

## Image
`04_ec2_deployment_flow.png`
