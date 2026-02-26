# EC2 Summary (Short Overview)

Amazon EC2 (Elastic Compute Cloud) provides scalable virtual servers in the cloud.

It allows you to launch, manage, and scale compute resources without buying physical hardware.

---

## 🔹 What EC2 Provides

- Virtual machines (instances)
- Flexible instance types (CPU, RAM, storage)
- Pay-as-you-go pricing
- Global deployment across regions

---

## 🔹 Core Components

- **AMI** → Operating system template
- **Instance Type** → Hardware configuration
- **EBS** → Block storage for instances
- **Security Groups** → Virtual firewall
- **Key Pair** → Secure SSH/RDP access
- **IAM Role** → Secure access to AWS services

---

## 🔹 Purchasing Options

- On-Demand → Flexible, no commitment
- Reserved / Savings Plans → Discounted, long-term
- Spot → Cheapest, interruptible
- Dedicated → Physical server for compliance

---

## 🔹 Security

- Security Groups control network access
- IAM Roles provide temporary credentials
- Customer manages OS patches and applications
- AWS manages physical infrastructure

---

## 🔹 Common Ports

- 22 → SSH
- 80 → HTTP
- 443 → HTTPS
- 3389 → RDP

---

## 🎯 Key Takeaways

- EC2 = Virtual server in AWS
- Choose instance type based on workload
- Use IAM Roles instead of access keys
- Open only required ports
- Understand pricing models for cost optimization
- Follow Shared Responsibility Model

---

EC2 is the foundation of compute services in AWS and a core topic for the Cloud Practitioner exam.