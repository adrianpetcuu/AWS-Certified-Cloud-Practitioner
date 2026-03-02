# Elastic Load Balancing (ELB) – Short Overview

Elastic Load Balancing (ELB) automatically distributes incoming traffic across multiple targets such as EC2 instances, containers, or IP addresses.

It improves:

- High Availability
- Fault tolerance
- Scalability

---

## 🔹 Why Use ELB?

Without a Load Balancer:
- All traffic goes to one server
- If that server fails → application goes down

With ELB:
- Traffic is distributed across multiple servers
- If one fails → traffic is redirected automatically

---

## 🔹 Types of Load Balancers

### 1️⃣ Application Load Balancer (ALB)
- Layer 7 (HTTP/HTTPS)
- Most commonly used
- Supports path-based routing (e.g., /api, /images)
- Used for web applications and microservices

---

### 2️⃣ Network Load Balancer (NLB)
- Layer 4 (TCP/UDP)
- Very high performance
- Low latency
- Used for extreme performance workloads

---

### 3️⃣ Gateway Load Balancer (GLB)
- Used for network appliances (firewalls, security tools)

---

## 🔹 How ELB Works

1. User sends request
2. Load Balancer receives traffic
3. ELB forwards traffic to healthy targets
4. Health checks monitor instance status

Only healthy instances receive traffic.

---

## 🔹 Key Components

- Load Balancer
- Target Group
- Listeners (port rules)
- Health Checks

---

## 🎯 Exam Key Points

- ELB improves High Availability
- Works across multiple Availability Zones
- Automatically distributes traffic
- Uses health checks
- ALB is most commonly tested

---

## Summary

Elastic Load Balancing ensures applications remain available, scalable, and fault-tolerant by distributing traffic across multiple resources.