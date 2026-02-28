# Amazon EFS (Elastic File System) – Short Overview

Amazon EFS provides **scalable file storage** for EC2 instances.

It is a fully managed **network file system (NFS)**.

---

## 🔹 What Is EFS?

- Shared file system
- Accessible by multiple EC2 instances at the same time
- Automatically scales storage up and down

---

## 🔹 Key Features

- Works across multiple Availability Zones
- Highly available and durable
- Fully managed by AWS
- No need to provision storage size manually

---

## 🔹 When to Use EFS

- Shared file storage between servers
- Web servers needing shared content
- Content management systems
- Home directories
- Big data workloads

---

## 🔹 EFS vs EBS

**EFS**
- File storage
- Shared across multiple instances
- Multi-AZ

**EBS**
- Block storage
- Attached to one instance (usually)
- Single AZ

---

## 🎯 Exam Key Points

- EFS = Managed file storage
- Supports multiple EC2 instances
- Scales automatically
- Multi-AZ

---

## Summary

Amazon EFS is a scalable, shared file system for EC2 that supports multiple instances and provides high availability across Availability Zones.