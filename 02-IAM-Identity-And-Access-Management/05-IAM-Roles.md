# IAM Roles (Short Overview)

## What is an IAM Role?

An **IAM Role** is an identity in AWS that provides **temporary permissions** to access AWS resources.

Unlike IAM users, a role:
- Does NOT have a password
- Does NOT have permanent access keys
- Uses temporary security credentials

---

## Why IAM Roles Are Important

IAM Roles are the **secure way** to grant access between AWS services.

Instead of storing access keys inside applications or servers, you assign a role.

---

## Common Use Cases

### 1️⃣ EC2 Instance Accessing S3
An EC2 instance can assume a role that allows it to:
- Read from S3
- Write to DynamoDB
- Access other AWS services

No access keys are stored on the server.

---

### 2️⃣ Lambda Accessing Other Services
A Lambda function uses a role to:
- Access databases
- Write logs to CloudWatch
- Read from S3

---

### 3️⃣ Cross-Account Access
A role can allow users from another AWS account to access specific resources.

---

## How IAM Roles Work

1. A role is created.
2. A policy is attached to the role.
3. The role is assigned to a service or assumed by a user.
4. AWS provides **temporary credentials** automatically.

---

## Benefits of IAM Roles

- More secure than access keys
- No credential management needed
- Automatic credential rotation
- Follows the Principle of Least Privilege

---

## Exam Key Points

- Roles provide **temporary credentials**
- Used by AWS services (EC2, Lambda, etc.)
- More secure than hardcoding access keys
- Essential for cross-account access