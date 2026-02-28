# EBS Snapshots (Short Overview)

An **EBS Snapshot** is a backup of an EBS volume.

Snapshots are stored in **Amazon S3** and can be used to restore or create new EBS volumes.

---

## 🔹 What Are Snapshots Used For?

- Backups
- Disaster recovery
- Creating new volumes
- Migrating data between Availability Zones or Regions

---

## 🔹 How They Work

- Snapshots are **incremental**
- Only changed blocks are saved after the first snapshot
- This reduces storage cost

---

## 🔹 Important Characteristics

- Stored in S3 (managed by AWS)
- Can be copied to another region
- Can be used to create a new EBS volume
- Can encrypt volumes during restore

---

## 🔹 Backup Strategy

Common approach:
1. Create snapshot
2. Store in S3 (automatically)
3. Restore when needed

---

## 🎯 Exam Key Points

- Snapshots are incremental
- Stored in S3
- Used for backup and recovery
- Can copy across regions
- Used to create new volumes

---

## Summary

EBS Snapshots provide a reliable way to back up and restore EC2 storage, supporting high availability and disaster recovery strategies.