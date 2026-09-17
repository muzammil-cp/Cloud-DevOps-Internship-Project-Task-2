# Security Groups

## Objective

Configure network access rules for the EC2 web server.

## Requirements

- Amazon EC2
- Security Group
- SSH
- HTTP
- HTTPS

## Configuration

Security Group name:

`web-server-sg`

### Inbound Rules

| Protocol | Port | Source | Purpose |
|---|---:|---|---|
| SSH | 22 | My IP | Server administration |
| HTTP | 80 | 0.0.0.0/0 | Web access |
| HTTPS | 443 | 0.0.0.0/0 | Secure web access |

SSH access is restricted to the administrator's IP address rather than being open to the entire Internet.

## Commands

Verify security groups:

```bash
aws ec2 describe-security-groups
