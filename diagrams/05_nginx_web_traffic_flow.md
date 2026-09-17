# 05 — Nginx Web Traffic Flow

## Objective
Show how web traffic reaches the Nginx server running on EC2.

## Configuration
- HTTP: port `80`
- HTTPS: port `443` where configured
- Nginx running on Ubuntu EC2
- SSH restricted to the administrator IP

## Verification

```bash
sudo systemctl status nginx
curl http://localhost
```

Then open:

```text
http://YOUR_EC2_PUBLIC_IP
```

## Image
`05_nginx_web_traffic_flow.png`
