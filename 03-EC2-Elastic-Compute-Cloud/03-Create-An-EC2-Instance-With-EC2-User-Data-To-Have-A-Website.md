# Create an EC2 Instance with EC2 User Data to Host a Website (Short Overview)

You can automatically install and configure a web server on an EC2 instance using **User Data**.

User Data is a script that runs automatically when the instance launches for the first time.

---

## What Is User Data?

User Data is a startup script (usually Bash for Linux) that:

- Installs software
- Updates packages
- Configures services
- Creates files (like an HTML page)

It runs automatically at first boot.

---

## Basic Steps

1️⃣ Launch a new EC2 instance  
2️⃣ Choose an AMI (e.g., Amazon Linux)  
3️⃣ Choose an instance type (e.g., t2.micro)  
4️⃣ Configure Security Group:
   - Allow HTTP (port 80)
5️⃣ In the **User Data** section, add a script
6️⃣ Launch the instance

---

## Example User Data Script (Amazon Linux)

```bash
#!/bin/bash
yum update -y
yum install -y httpd
systemctl start httpd
systemctl enable httpd
echo "<h1>My Website is Running!</h1>" > /var/www/html/index.html
```

## What Happens?

The instance launches

Apache (httpd) installs automatically

Web server starts

A simple website is created

You access it via the public IP

## Important Notes

Make sure port 80 is open in the Security Group

User Data runs only at first launch (by default)

The instance must have a public IP to be accessible from the internet

## Summary

Using EC2 User Data allows you to:

Automate server setup

Deploy websites instantly

Avoid manual configuration

Follow Infrastructure as Code principles