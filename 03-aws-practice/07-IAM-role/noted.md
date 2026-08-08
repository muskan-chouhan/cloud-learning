# AWS IAM (Identity and Access Management)

## What is IAM?

IAM (Identity and Access Management) is an AWS service used to securely manage:

- Users
- Groups
- Roles
- Permissions
- Policies

IAM controls **who can access which AWS resources**.

---

# Why IAM?

Without IAM:

- Everyone would use the root account.
- High security risk.
- No access control.

IAM allows us to follow the **Principle of Least Privilege** by giving only the required permissions.

---
  
# IAM Components 

## 1. Root User

- Created when AWS account is created.
- Has full access to all AWS services.
- Should not be used for daily work.

Best Practice:

- Enable MFA
- Create IAM Users
- Avoid using Root Account

---

## 2. IAM User

Represents an individual person.

Example:

- Cloud Admin
- Developer
- Dev