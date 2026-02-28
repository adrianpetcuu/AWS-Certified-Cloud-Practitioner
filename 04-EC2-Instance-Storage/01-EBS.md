# Amazon EBS (Elastic Block Store) – Short Overview

Amazon EBS provides **block storage** for EC2 instances.

It works like a virtual hard drive that you attach to a server.

---

## 🔹 What Is EBS?

- Persistent storage for EC2
- Data remains even if the instance is stopped
- Can be attached to one EC2 instance at a time (in most cases)

---

## 🔹 Key Features

- Highly available within one Availability Zone
- Automatically replicated inside the AZ
- Can create snapshots (backups)
- Can increase size without losing data

---

## 🔹 EBS vs Instance Store

**EBS**
- Persistent
- Data survives stop/start
- Can be backed up

**Instance Store**
- Temporary
- Data lost if instance stops or terminates

---

## 🔹 Common EBS Volume Types

- **gp2 / gp3** → General Purpose (most common)
- **io1 / io2** → High performance
- **st1** → Throughput optimized
- **sc1** → Cold HDD (low cost)

For most workloads:
👉 Use gp3

---

## 🔹 Snapshots

- Stored in S3
- Used for backups
- Can restore new volumes from snapshots

---

## 🎯 Exam Key Points

- EBS = Block storage for EC2
- Persistent storage
- AZ-specific
- Supports snapshots
- gp3 is default recommended type

---

## Summary

Amazon EBS provides reliable, persistent block storage for EC2 instances and is essential for storing operating systems, databases, and application data.