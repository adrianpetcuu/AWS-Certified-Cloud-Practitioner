# EC2 Instance Roles (Short Overview)

## What Is an EC2 Instance Role?

An **EC2 Instance Role** is an IAM Role attached to an EC2 instance.

It allows the instance to securely access other AWS services **without using access keys**.

---

## Why It Is Important

Instead of storing:
- Access Key ID
- Secret Access Key

inside your server, you assign a role.

AWS automatically provides **temporary credentials** to the instance.

---

## Common Use Cases

- EC2 reading from S3
- EC2 writing to DynamoDB
- EC2 sending logs to CloudWatch
- EC2 accessing other AWS services

---

## How It Works

1️⃣ Create an IAM Role  
2️⃣ Attach a policy (define permissions)  
3️⃣ Assign the role to the EC2 instance  
4️⃣ AWS provides temporary credentials automatically  

No manual key management required.

---

## Benefits

- More secure than access keys
- Automatic credential rotation
- Follows Least Privilege principle
- No hardcoded secrets

---

## Exam Key Points

- EC2 uses **IAM Roles**, not access keys
- Roles provide **temporary credentials**
- Best practice for service-to-service access

---

## Summary

EC2 Instance Roles allow EC2 instances to securely access AWS services using temporary credentials instead of permanent access keys.