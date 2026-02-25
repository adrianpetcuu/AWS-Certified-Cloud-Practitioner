# IAM Introduction – Users, Groups, Policies

AWS Identity and Access Management (IAM) controls **who can access AWS resources** and **what actions they can perform**.

IAM is a core security service in AWS and follows the principle of least privilege.

---

## 1️⃣ IAM Users

An **IAM User** represents a person or an application that needs access to AWS.

A user can have:
- Username
- Password (for AWS Console access)
- Access Keys (for CLI / SDK access)

### Example:
- developer1
- admin-user
- backend-app

Best Practice:
> Do not use the root account for daily activities. Create IAM users instead.

---

## 2️⃣ IAM Groups

An **IAM Group** is a collection of IAM users.

Groups are used to assign permissions to multiple users at once.

### Example:
- Developers
- Admins
- ReadOnlyUsers

Instead of attaching permissions to each user individually, attach them to a group.

Best Practice:
> Assign permissions to groups, then add users to those groups.

---

## 3️⃣ IAM Policies

An **IAM Policy** defines permissions.

Policies are written in JSON format and control:

- **Effect** → Allow or Deny
- **Action** → What action is allowed (e.g., `s3:ListBucket`)
- **Resource** → Which resource the action applies to

### Simple Example:

```json
{
  "Effect": "Allow",
  "Action": "s3:ListBucket",
  "Resource": "*"
}
```

Important Rules:

Explicit Deny overrides Allow

Always follow the Principle of Least Privilege

🔐 Summary

Users → Individual identities

Groups → Collection of users

Policies → Permission rules

IAM ensures secure and controlled access to AWS resources.