# EC2 Instance Types – Basics (Short Overview)

EC2 Instance Types define the **hardware configuration** of your virtual server.

They determine:
- CPU power
- Memory (RAM)
- Storage performance
- Network capacity

---

## 🧩 Instance Naming Example

Example: `t3.micro`

Breakdown:
- **t** → Instance family
- **3** → Generation
- **micro** → Size (CPU/RAM capacity)

---

## 🗂️ Main Instance Families

### 1️⃣ General Purpose (Balanced)
Balanced CPU, memory, networking.

Examples:
- t (t2, t3)
- m (m5, m6)

Use cases:
- Web servers
- Small databases
- Development environments

---

### 2️⃣ Compute Optimized
High CPU performance.

Examples:
- c family

Use cases:
- Batch processing
- High-performance computing
- Game servers

---

### 3️⃣ Memory Optimized
High RAM.

Examples:
- r family

Use cases:
- In-memory databases
- Big data processing

---

### 4️⃣ Storage Optimized
High disk performance.

Examples:
- i family

Use cases:
- Large databases
- Data warehousing

---

## 🆓 Free Tier

Free Tier eligible:
- `t2.micro`
- `t3.micro` (depending on region)

---

## 📌 Key Points for Exam

- Choose instance type based on workload.
- Compute optimized = more CPU.
- Memory optimized = more RAM.
- General purpose = balanced.
- Instance type impacts cost.

---

## 🎯 Summary

EC2 Instance Types define the performance and cost of your server.

Select the instance family based on:
- CPU needs
- Memory requirements
- Storage performance
- Budget