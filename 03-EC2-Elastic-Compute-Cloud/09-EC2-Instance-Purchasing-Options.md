# EC2 Instance Purchasing Options (Short Overview)

AWS offers multiple purchasing options for EC2 instances depending on cost and usage needs.

---

## 1️⃣ On-Demand Instances

- Pay per hour or per second
- No long-term commitment
- Flexible and easy to start

Best for:
- Short-term workloads
- Testing
- Unpredictable traffic

💰 Highest cost compared to other options.

---

## 2️⃣ Reserved Instances (RI)

- 1-year or 3-year commitment
- Significant discount (up to ~72%)
- Can choose partial or full upfront payment

Best for:
- Steady, predictable workloads
- Long-term production systems

💡 Lower cost but less flexible.

---

## 3️⃣ Savings Plans

- Commit to a consistent usage amount ($/hour)
- Flexible across instance families and regions
- Discount similar to Reserved Instances

Best for:
- Long-term usage with flexibility

---

## 4️⃣ Spot Instances

- Use unused AWS capacity
- Up to 90% cheaper than On-Demand
- Can be interrupted anytime

Best for:
- Batch jobs
- Big data
- Fault-tolerant workloads

⚠️ Not suitable for critical applications.

---

## 5️⃣ Dedicated Hosts / Dedicated Instances

- Physical server dedicated to you
- Required for compliance or licensing

Most expensive option.

---

## 🎯 Exam Key Points

- On-Demand → flexible, no commitment
- Reserved / Savings Plans → cheaper, long-term commitment
- Spot → cheapest, can be interrupted
- Choose based on workload stability and cost needs

---

## Summary

EC2 purchasing options allow you to balance:
- Cost
- Flexibility
- Reliability
- Commitment duration