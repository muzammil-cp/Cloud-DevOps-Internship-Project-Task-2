# Nginx Deployment

## Objective

Install and verify Nginx as the web server on the Ubuntu EC2 instance.

## Configuration

Nginx was installed on the Ubuntu EC2 instance and configured to start automatically.

## Commands

Update packages:

```bash
sudo apt update
```

Install Nginx:

```bash
sudo apt install nginx -y
```

Check the service:

```bash
sudo systemctl status nginx
```

Test locally:

```bash
curl http://localhost
```

## Verification

The Nginx default page and custom webpage were verified from the browser.

## Evidence

- `screenshots/11.1_nginx_default_page.png`
- `screenshots/12.1_nginx_browser.png`
- `screenshots/13.1_custom_nginx_page.png`
