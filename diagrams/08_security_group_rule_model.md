# 08 — Security Group Rule Model

## Objective
Document the network access rules for the EC2 web server.

## Inbound Rules

| Protocol | Port | Source | Purpose |
|---|---:|---|---|
| SSH | 22 | My IP | Administration |
| HTTP | 80 | 0.0.0.0/0 | Web access |
| HTTPS | 443 | 0.0.0.0/0 | HTTPS access |

## Verification

```bash
aws ec2 describe-security-groups
```

On Ubuntu:

```bash
sudo ss -tulnp
```

## Security
SSH should not be opened to `0.0.0.0/0` for this lab when a restricted administrator IP can be used.

## Image
`08_security_group_rule_model.png`
