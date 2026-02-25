# IAM Summary (Short Overview)

AWS Identity and Access Management (IAM) controls **who can access AWS resources** and **what actions they can perform**.

---

## 🔑 Core Components

- **Users** → Individual identities (people or applications)
- **Groups** → Collection of users with shared permissions
- **Roles** → Temporary identities used by AWS services or for cross-account access
- **Policies** → JSON documents that define permissions (Allow / Deny)

---

## 🔐 Security Concepts

- **Authentication** → Proving identity (password, MFA, access keys)
- **Authorization** → Determining what actions are allowed
- **MFA** → Adds an extra layer of security
- **Least Privilege** → Grant only required permissions

---

## ⚙️ Programmatic Access

- **Access Keys** → Used for CLI and SDK
- **IAM Roles** → Preferred over permanent access keys
- **Temporary credentials** → More secure and auto-rotated

---

## 📊 Monitoring & Control

- **CloudTrail** → Tracks API activity
- **Credential Report** → Audits IAM users
- **Access Advisor** → Identifies unused permissions

---

## 🎯 Key Takeaway

IAM ensures secure and controlled access to AWS by managing:

- Identities
- Permissions
- Authentication methods
- Security best practices