# AWS Budget Setup (Short Overview)

AWS Budgets allows you to monitor your AWS costs and receive alerts when spending exceeds defined limits.

It helps you avoid unexpected charges and stay within your planned budget.

---

## What Is AWS Budgets?

AWS Budgets is a cost management tool that lets you:

- Set custom cost or usage limits
- Track spending over time
- Receive alerts when thresholds are reached

---

## Types of Budgets

1️⃣ **Cost Budget**  
Monitor total AWS spending.

2️⃣ **Usage Budget**  
Track usage of services (e.g., hours of EC2).

3️⃣ **Savings Plans / Reservation Budget**  
Track commitment-based usage.

---

## How to Create a Budget (Basic Steps)

1. Go to **Billing & Cost Management**
2. Select **Budgets**
3. Click **Create budget**
4. Choose budget type (Cost recommended)
5. Set:
   - Budget amount (e.g., $20/month)
   - Time period (Monthly)
6. Configure alerts (e.g., 80%, 100%)
7. Add email for notifications
8. Create budget

---

## Why It Is Important

- Prevents unexpected bills
- Helps control cloud spending
- Especially important for Free Tier users

---

## Best Practice

- Always create a budget when starting with AWS
- Set alerts at 50%, 80%, and 100%
- Monitor usage regularly

---

## Summary

AWS Budgets helps you:
- Control costs
- Receive alerts
- Stay within spending limits