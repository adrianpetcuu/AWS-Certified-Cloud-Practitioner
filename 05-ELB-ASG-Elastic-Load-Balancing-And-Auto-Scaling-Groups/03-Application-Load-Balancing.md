# Application Load Balancer (ALB) – Short Overview

Application Load Balancer (ALB) is a Layer 7 load balancer that distributes HTTP and HTTPS traffic across multiple targets.

It is part of Elastic Load Balancing (ELB).

---

## 🔹 What Makes ALB Special?

ALB works at the **application layer (Layer 7)** and understands:

- HTTP
- HTTPS
- URLs
- Hostnames

It can route traffic based on rules.

---

## 🔹 Key Features

- Path-based routing  
  Example:  
  `/api` → Server Group A  
  `/images` → Server Group B  

- Host-based routing  
  Example:  
  `api.example.com` → Backend A  
  `app.example.com` → Backend B  

- Integrated with Auto Scaling
- Performs health checks
- Supports SSL/TLS (HTTPS)

---

## 🔹 How It Works

1. User sends HTTP/HTTPS request
2. ALB receives traffic
3. ALB checks routing rules
4. Forwards request to a healthy target in a Target Group

---

## 🔹 When to Use ALB

- Web applications
- Microservices architectures
- REST APIs
- Applications requiring advanced routing

---

## 🎯 Exam Key Points

- ALB = Layer 7
- Works with HTTP/HTTPS
- Supports path and host-based routing
- Uses Target Groups
- Performs health checks
- Works with Auto Scaling

---

## Summary

Application Load Balancer distributes web traffic intelligently, improves availability, and enables advanced routing for modern cloud applications.