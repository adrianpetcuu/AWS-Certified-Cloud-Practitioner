# 6️⃣ Shared Responsibility Model & AWS Acceptable Use Policy

Understanding security responsibilities is fundamental in AWS.

Security in the cloud is based on a **Shared Responsibility Model**, and usage of AWS services is governed by the **AWS Acceptable Use Policy (AUP)**.

---

# Shared Responsibility Model

AWS security is divided between:

- **Security OF the Cloud** → Responsibility of AWS  
- **Security IN the Cloud** → Responsibility of the Customer  

---

## 1️⃣ Security OF the Cloud (AWS Responsibility)

AWS is responsible for protecting the infrastructure that runs all AWS services.

This includes:

- Physical data centers
- Hardware
- Networking infrastructure
- Storage devices
- Global backbone network
- Virtualization layer

AWS ensures:

- Physical security
- Environmental controls
- Hardware maintenance
- Infrastructure compliance certifications

You do NOT manage these components.

---

## 2️⃣ Security IN the Cloud (Customer Responsibility)

Customers are responsible for what they deploy and configure inside AWS.

This includes:

- Data protection
- Identity and access management
- Operating system updates
- Application security
- Firewall configuration
- Encryption settings
- Network configuration

If you misconfigure a service, it is your responsibility.

---

# Responsibility Depends on Service Type

The level of responsibility varies based on the service model:

### IaaS (Infrastructure as a Service)

You manage:
- Operating system
- Applications
- Data
- Security configurations

AWS manages:
- Physical infrastructure
- Virtualization
- Hardware

---

### PaaS (Platform as a Service)

You manage:
- Application code
- Data

AWS manages:
- OS
- Runtime
- Infrastructure

---

### SaaS (Software as a Service)

You manage:
- Data access
- User permissions

AWS manages:
- Almost everything else

---

# Why the Shared Responsibility Model Matters

Understanding this model helps you:

- Avoid security misconfigurations
- Prepare for compliance audits
- Define internal security policies
- Design secure architectures

A common misconception:
"Security in AWS is fully handled by AWS."

This is incorrect. AWS secures the infrastructure, but you must secure your workloads.

---

# AWS Acceptable Use Policy (AUP)

The AWS Acceptable Use Policy defines how customers are allowed to use AWS services.

It exists to:

- Protect AWS infrastructure
- Prevent abuse
- Maintain service integrity

---

## Prohibited Activities (Examples)

You are NOT allowed to use AWS for:

- Illegal activities
- Distributing malware
- Hosting phishing websites
- Sending spam
- Launching DDoS attacks
- Attempting to breach systems
- Mining cryptocurrency in restricted ways (depending on terms)
- Violating intellectual property rights

---

## What Happens if You Violate the AUP?

AWS may:

- Suspend resources
- Restrict account access
- Terminate services
- Report illegal activity

Compliance with the AUP is mandatory for all AWS customers.

---

# Key Takeaways

- AWS secures the infrastructure.
- You secure your data, applications, and configurations.
- Responsibilities vary depending on the service model (IaaS, PaaS, SaaS).
- The Acceptable Use Policy defines what is allowed and prohibited on AWS.

Understanding both concepts is essential for passing the AWS Certified Cloud Practitioner exam and for building secure cloud architectures.