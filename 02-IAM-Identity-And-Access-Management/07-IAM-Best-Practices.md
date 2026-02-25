# IAM Best Practices (Short Overview)

Following IAM best practices helps secure your AWS environment and reduce security risks.

---

## 1️⃣ Do NOT Use the Root Account Daily

- Use root only for account setup and critical tasks.
- Enable **MFA** on the root account.
- Create IAM users for regular work.

---

## 2️⃣ Apply the Principle of Least Privilege

Grant only the permissions required to perform a task.

- Avoid giving full administrative access.
- Remove unused permissions regularly.

---

## 3️⃣ Use IAM Groups

- Assign permissions to groups.
- Add users to groups.
- Avoid attaching policies directly to individual users.

---

## 4️⃣ Use IAM Roles Instead of Access Keys

- Assign roles to EC2, Lambda, and other services.
- Avoid hardcoding access keys.
- Prefer temporary credentials.

---

## 5️⃣ Enable Multi-Factor Authentication (MFA)

- Required for root account.
- Recommended for admin users.
- Adds an extra security layer.

---

## 6️⃣ Rotate and Monitor Credentials

- Rotate access keys regularly.
- Remove unused users and keys.
- Review IAM Credential Reports.

---

## 7️⃣ Monitor Activity

- Use CloudTrail to track API calls.
- Audit IAM activity regularly.

---

## 🎯 Summary

IAM Best Practices focus on:

- Least privilege
- Strong authentication (MFA)
- Role-based access
- Monitoring and auditing
- Minimizing permanent credentials