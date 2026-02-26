# EC2 Basics (Short Overview)

Amazon EC2 (Elastic Compute Cloud) provides **virtual servers in the cloud**.

You can launch, configure, and manage servers without buying physical hardware.

---

## What Is an EC2 Instance?

An EC2 instance is a virtual machine that runs:

- An operating system (Linux or Windows)
- Applications
- Databases
- Web servers

You pay only for the time the instance is running.

---

## Key Components When Launching an EC2 Instance

1️⃣ **AMI (Amazon Machine Image)**  
Defines the operating system and initial software.  
Examples: Amazon Linux, Ubuntu, Windows.

2️⃣ **Instance Type**  
Defines CPU, RAM, and network performance.  
Example: t2.micro (Free Tier eligible).

3️⃣ **Storage (EBS)**  
Elastic Block Store volume attached to the instance.

4️⃣ **Security Group**  
Acts as a firewall controlling inbound and outbound traffic.

5️⃣ **Key Pair**  
Used to securely connect via SSH (Linux) or RDP (Windows).

---

## Common Ports

- 22 → SSH (Linux access)
- 80 → HTTP (Web traffic)
- 443 → HTTPS (Secure web)
- 3389 → RDP (Windows access)

---

## Important Concepts

- Instances are region-specific.
- Stopped instances do not incur compute charges (but storage still costs).
- Security Groups are stateful firewalls.

---

## Summary

EC2 allows you to:

- Launch virtual servers quickly
- Scale compute resources
- Pay only for what you use
- Control access through Security Groups and IAM