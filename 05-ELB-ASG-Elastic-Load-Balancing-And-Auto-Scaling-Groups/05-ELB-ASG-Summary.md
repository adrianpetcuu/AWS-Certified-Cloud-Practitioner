# ELB & ASG Summary (Short Overview)

Elastic Load Balancing (ELB) and Auto Scaling Groups (ASG) work together to provide:

- High Availability
- Scalability
- Elasticity
- Cost optimization

---

## 🔹 Elastic Load Balancing (ELB)

ELB distributes incoming traffic across multiple EC2 instances.

Key Points:
- Improves availability
- Performs health checks
- Sends traffic only to healthy instances
- Works across multiple Availability Zones

Most common type:
- Application Load Balancer (ALB) – Layer 7 (HTTP/HTTPS)

---

## 🔹 Auto Scaling Groups (ASG)

ASG automatically adjusts the number of EC2 instances based on demand.

Key Points:
- Maintains minimum, maximum, and desired capacity
- Replaces unhealthy instances
- Scales automatically using CloudWatch metrics
- Reduces costs during low traffic

---

## 🔹 How They Work Together

1. User sends request
2. ELB receives traffic
3. ELB forwards to healthy EC2 instances
4. ASG adds or removes instances based on load

Together they provide:
- Fault tolerance
- Automatic scaling
- Better performance
- Reduced downtime

---

## 🎯 Exam Key Takeaways

- ELB = Traffic distribution
- ASG = Automatic scaling
- Use together for High Availability and Elasticity
- Multi-AZ deployment is best practice

---

## Final Summary

ELB handles traffic.  
ASG manages capacity.  
Together, they ensure scalable and highly available cloud applications.