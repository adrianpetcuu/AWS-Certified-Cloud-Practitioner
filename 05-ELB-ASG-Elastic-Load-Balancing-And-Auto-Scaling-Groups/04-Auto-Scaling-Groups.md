# Auto Scaling Groups (ASG) – Short Overview

Auto Scaling Groups (ASG) automatically manage a group of EC2 instances.

They ensure:

- High Availability
- Automatic scaling
- Cost optimization

---

## 🔹 What Does an ASG Do?

- Launches EC2 instances
- Terminates instances when not needed
- Replaces unhealthy instances automatically
- Scales based on demand

---

## 🔹 Key Parameters

When creating an ASG, you define:

- **Minimum capacity** → Minimum number of instances
- **Maximum capacity** → Maximum allowed instances
- **Desired capacity** → Target number of running instances

Example:
Min: 2  
Desired: 2  
Max: 6  

---

## 🔹 Scaling Policies

### 1️⃣ Target Tracking (Most Common)
Maintains a metric at a specific value.
Example:
- Keep CPU at 50%

### 2️⃣ Step Scaling
Adds or removes instances based on thresholds.

### 3️⃣ Scheduled Scaling
Scales at specific times (e.g., business hours).

---

## 🔹 Integration with Load Balancer

ASG works with ELB:

- ELB distributes traffic
- ASG adjusts number of instances
- Only healthy instances receive traffic

---

## 🎯 Exam Key Points

- ASG maintains desired number of instances
- Automatically replaces failed instances
- Supports automatic scaling
- Works with CloudWatch metrics
- Commonly used with Load Balancers

---

## Summary

Auto Scaling Groups automatically adjust the number of EC2 instances to maintain performance, availability, and cost efficiency.