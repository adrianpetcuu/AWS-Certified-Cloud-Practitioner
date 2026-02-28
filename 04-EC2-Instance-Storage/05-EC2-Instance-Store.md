# EC2 Instance Store – Short Overview

**EC2 Instance Store** provides temporary block storage that is physically attached to the host machine.

It is also called **ephemeral storage**.

---

## 🔹 Key Characteristics

- Temporary storage
- Data is lost if the instance:
  - Stops
  - Terminates
  - Fails

- High performance
- Physically attached to the host

---

## 🔹 When to Use It

Suitable for:

- Cache
- Buffers
- Temporary files
- Scratch data
- Applications that can tolerate data loss

Not suitable for:

- Databases
- Critical data
- Long-term storage

---

## 🔹 Instance Store vs EBS

**Instance Store**
- Temporary
- Data lost on stop/terminate
- High performance

**EBS**
- Persistent
- Data survives stop/start
- Can create snapshots

---

## 🎯 Exam Key Points

- Instance Store = temporary storage
- Data lost when instance stops or terminates
- Good for non-critical, high-performance workloads

---

## Summary

EC2 Instance Store provides fast, temporary storage attached to the host machine and should only be used for data that does not need to be persistent.