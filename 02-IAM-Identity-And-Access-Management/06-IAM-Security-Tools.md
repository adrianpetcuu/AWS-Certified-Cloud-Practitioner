# IAM Security Tools (Short Overview)

AWS provides several tools to help monitor and improve IAM security.

---

## 1️⃣ IAM Credential Report

Generates a report of all IAM users in your account.

Shows:
- Password usage
- MFA enabled or not
- Access key age
- Last login time

Useful for:
- Security audits
- Checking unused credentials
- Ensuring MFA is enabled

---

## 2️⃣ IAM Access Advisor

Shows which AWS services a user, group, or role has accessed.

Helps you:
- Identify unused permissions
- Apply the Principle of Least Privilege
- Remove unnecessary access

---

## 3️⃣ AWS CloudTrail

Records API calls and account activity.

Tracks:
- Who did what
- When
- From where

Used for:
- Auditing
- Compliance
- Security investigations

---

## 4️⃣ AWS Trusted Advisor (Security Checks)

Provides recommendations such as:
- Enable MFA on root account
- Remove unused IAM users
- Rotate access keys

---

## 🎯 Summary

IAM Security Tools help you:
- Monitor access
- Audit user activity
- Reduce excessive permissions
- Improve overall cloud security posture