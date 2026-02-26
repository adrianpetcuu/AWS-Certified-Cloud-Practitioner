# Shared Responsibility Model for EC2 (Short Overview)

When using Amazon EC2, security responsibilities are shared between AWS and the customer.

---

## 🔹 AWS Responsibility (Security OF the Cloud)

AWS is responsible for:

- Physical data centers
- Hardware (servers, storage, networking)
- Hypervisor (virtualization layer)
- Global infrastructure
- Power and cooling

You do NOT manage these components.

---

## 🔹 Customer Responsibility (Security IN the Cloud)

You are responsible for everything inside the EC2 instance, including:

- Operating system updates and patches
- Application security
- Firewall configuration (Security Groups)
- Network configuration
- IAM roles and permissions
- Data encryption
- Antivirus (if needed)

If your EC2 server is hacked due to weak passwords or unpatched OS, it is your responsibility.

---

## 🔐 Example

AWS secures:
- The physical server running your instance.

You secure:
- The Linux/Windows OS.
- Installed software.
- Open ports (22, 80, etc.).

---

## 🎯 Exam Key Idea

- AWS secures the infrastructure.
- You secure the operating system and applications.

---

## Summary

With EC2:

AWS = Hardware & infrastructure security  
Customer = OS, applications, data, and access management