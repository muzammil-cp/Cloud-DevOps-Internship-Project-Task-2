# Security Groups

## Objective

Configure network access rules for the EC2 web server.

## Configuration

```text
Security Group: web-server-sg
```

### Inbound Rules

| Protocol | Port | Source | Purpose |
|---|---:|---|---|
| SSH | 22 | My IP | Server administration |
| HTTP | 80 | 0.0.0.0/0 | Web access |
| HTTPS | 443 | 0.0.0.0/0 | Secure web access |

SSH access should be restricted to the administrator's IP rather than being open to the entire Internet.

## Verification

```bash
aws ec2 describe-security-groups
```

On Ubuntu:

```bash
sudo ss -tulnp
```

## Evidence

- `screenshots/08.1_security_group.png`
