# 05 — Nginx Web Traffic Flow

## Objective

Document the path from Internet traffic to the Nginx web server.

## Flow

```text
Internet
   |
Internet Gateway
   |
Public Subnet
   |
Security Group
   |
EC2
   |
Nginx
```

## HTTP Verification

```text
the EC2 instance's current public IPv4 address
```

The actual public IP is intentionally not stored in the repository.

## Evidence

Nginx was verified using the browser and the EC2 instance.

## Image

`05_nginx_web_traffic_flow.png`
