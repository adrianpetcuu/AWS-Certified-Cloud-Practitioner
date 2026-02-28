# Shared Responsibility Model for EC2 Storage (Short Overview)

When using EC2 storage services (EBS, EFS, Instance Store), security responsibilities are shared between AWS and the customer.

---

## 🔹 AWS Responsibility (Security OF the Cloud)

AWS is responsible for:

- Physical data centers
- Storage hardware
- Disk durability and availability
- Replication within an Availability Zone (EBS)
- Multi-AZ design (EFS infrastructure)
- Infrastructure-level encryption support

You do NOT manage physical disks or data center security.

---

## 🔹 Customer Responsibility (Security IN the Cloud)

You are responsible for:

- Data encryption (enable EBS/EFS encryption)
- Managing IAM permissions
- Controlling access via Security Groups
- Configuring backups (EBS snapshots)
- Managing file system permissions (EFS)
- Protecting sensitive data

If data is exposed due to misconfigured permissions, it is your responsibility.

---

## 🔐 Example

AWS secures:
- The physical storage devices.

You secure:
- Who can access the volume.
- Whether encryption is enabled.
- Backup strategy.
- OS-level file permissions.

---

## 🎯 Exam Key Idea

AWS secures the infrastructure.

You secure:
- Data
- Access
- Encryption
- Backups

---

## Summary

For EC2 storage:

AWS = Physical storage & infrastructure  
Customer = Data protection, encryption, permissions, and backups