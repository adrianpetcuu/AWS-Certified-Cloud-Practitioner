# High Availability, Scalability & Elasticity (Short Overview)

These three concepts are fundamental in cloud architecture and are commonly tested in AWS exams.

---

## 🔹 High Availability (HA)

High Availability means a system remains operational even if part of the infrastructure fails.

### How it is achieved:
- Deploying resources in multiple Availability Zones (Multi-AZ)
- Using Load Balancers
- Having multiple EC2 instances

### Goal:
Minimize downtime and ensure continuous service.

---

## 🔹 Scalability

Scalability is the ability of a system to handle increased workload by adding resources.

### Types:

**1️⃣ Vertical Scaling**
- Increase CPU/RAM of an existing server
- Example: Upgrade from t3.micro to t3.large

**2️⃣ Horizontal Scaling**
- Add more servers
- Example: Add more EC2 instances behind a Load Balancer

---

## 🔹 Elasticity

Elasticity is the ability to automatically increase or decrease resources based on demand.

### Example:
- Traffic increases → Auto Scaling adds instances
- Traffic decreases → Auto Scaling removes instances

### Goal:
Optimize cost and performance dynamically.

---

## 🎯 Key Differences

- High Availability → Prevent downtime
- Scalability → Handle growth
- Elasticity → Automatically adjust to demand

---

## Summary

Cloud architecture focuses on:
- High Availability for reliability
- Scalability for growth
- Elasticity for cost-efficient automation