# EC2 Instance Storage Summary (Short Overview)

EC2 instances can use different types of storage depending on performance, persistence, and sharing requirements.

---

## 🔹 1️⃣ EBS (Elastic Block Store)

- Block storage
- Persistent (data survives stop/start)
- Attached to one instance (usually)
- AZ-specific
- Supports snapshots (backups)

Best for:
- Operating systems
- Databases
- Application data

---

## 🔹 2️⃣ Instance Store

- Temporary storage
- Data lost if instance stops or terminates
- High performance
- Physically attached to host

Best for:
- Cache
- Temporary files
- Non-critical data

---

## 🔹 3️⃣ EFS (Elastic File System)

- File storage (NFS)
- Shared across multiple EC2 instances
- Multi-AZ
- Automatically scales

Best for:
- Shared web content
- Content management systems
- File sharing

---

## 🔹 4️⃣ Amazon FSx

- Managed specialized file systems
- Windows File Server, Lustre, ONTAP, OpenZFS
- High-performance and enterprise workloads

Best for:
- Windows environments
- HPC
- Enterprise storage needs

---

## 🎯 Key Differences

| Storage Type   | Persistent | Shared | AZ Scope | Use Case |
|---------------|------------|--------|----------|----------|
| EBS           | Yes        | No     | Single AZ| OS & DB |
| Instance Store| No         | No     | Host-based| Cache |
| EFS           | Yes        | Yes    | Multi-AZ | Shared files |
| FSx           | Yes        | Yes    | Varies   | Specialized workloads |

---

## Summary

EC2 storage options allow you to choose between:

- Persistent vs temporary
- Block vs file storage
- Single-instance vs shared access
- General-purpose vs specialized performance

Select storage based on workload requirements and durability needs.