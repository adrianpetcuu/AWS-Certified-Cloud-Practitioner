# Security Groups – Classic Ports Overview (Short Overview)

A **Security Group** acts as a virtual firewall for EC2 instances.

It controls **inbound (incoming)** and **outbound (outgoing)** traffic.

Security Groups are **stateful**:
- If inbound traffic is allowed, the response is automatically allowed.
- You do not need to create separate outbound rules for responses.

---

## 🔐 Common (Classic) Ports

### 22 – SSH
- Used to connect to Linux instances.
- Protocol: TCP
- Should be restricted to your IP address.

---

### 80 – HTTP
- Standard web traffic (non-secure).
- Used to host websites.

---

### 443 – HTTPS
- Secure web traffic (encrypted).
- Recommended for production websites.

---

### 3389 – RDP
- Used to connect to Windows instances.
- Protocol: TCP
- Should be restricted to your IP address.

---

### 21 – FTP
- File transfer protocol.
- Less common today (often replaced by SFTP).

---

## 🌍 Source Options

When creating rules, you define the **source**:

- `0.0.0.0/0` → Allow traffic from anywhere (public internet)
- Your IP → Secure access (recommended for SSH/RDP)
- Another Security Group → Internal communication between instances

---

## ⚠️ Best Practices

- Do NOT open port 22 or 3389 to the whole internet.
- Use least privilege.
- Allow only required ports.
- Restrict access by IP when possible.

---

## 🎯 Summary

Security Groups control network access to EC2 instances.

Important ports to remember:
- 22 → SSH
- 80 → HTTP
- 443 → HTTPS
- 3389 → RDP

They are stateful and essential for securing AWS workloads.