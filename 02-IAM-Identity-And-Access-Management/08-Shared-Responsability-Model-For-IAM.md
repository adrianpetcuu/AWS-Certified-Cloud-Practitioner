# Shared Responsibility Model for IAM (Short Overview)

In AWS, security follows the **Shared Responsibility Model**.

For IAM specifically, responsibilities are divided between AWS and the customer.

---

## 🔹 AWS Responsibility (Security OF the Cloud)

AWS is responsible for:

- Protecting the IAM infrastructure
- Securing data centers
- Maintaining hardware and networking
- Securing the AWS global infrastructure
- Protecting the IAM service backend

You do NOT manage these components.

---

## 🔹 Customer Responsibility (Security IN the Cloud)

You are responsible for:

- Creating and managing IAM users
- Defining IAM roles
- Writing and attaching policies
- Enabling MFA
- Rotating access keys
- Following least privilege
- Monitoring account activity

If permissions are misconfigured, it is the customer’s responsibility.

---

## 🎯 Key Idea

AWS secures the IAM service itself.

You secure:
- Who has access
- What they can do
- How authentication is handled

---

## ✅ Exam Tip

- AWS = infrastructure security
- Customer = identity management and permissions configuration