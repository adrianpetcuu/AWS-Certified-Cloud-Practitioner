# EC2 Instance Connect (Short Overview)

## What Is EC2 Instance Connect?

EC2 Instance Connect allows you to connect to a Linux EC2 instance directly from the AWS Console using your browser.

You do not need:
- SSH installed locally
- A downloaded `.pem` key file
- Third-party tools (like PuTTY)

---

## How It Works

- Uses temporary SSH keys
- Authenticates through your IAM permissions
- Connects via browser-based terminal

It works only for:
- Amazon Linux
- Ubuntu (with proper configuration)

---

## Requirements

1️⃣ The instance must:
- Be running
- Have a public IP (or proper networking)

2️⃣ Security Group must allow:
- Port 22 (SSH)

3️⃣ IAM user must have permission:
- `ec2-instance-connect:SendSSHPublicKey`

---

## How To Use It

1. Go to EC2 → Instances
2. Select your instance
3. Click **Connect**
4. Choose **EC2 Instance Connect**
5. Click **Connect**

A browser terminal opens.

---

## Advantages

- No local setup required
- Uses temporary credentials
- More secure than sharing `.pem` files
- Quick and simple access

---

## Limitations

- Only works with supported AMIs
- Requires proper IAM permissions
- Needs SSH (port 22) open

---

## Summary

EC2 Instance Connect provides secure browser-based SSH access to Linux EC2 instances without managing key files locally.