![AWS](https://img.shields.io/badge/AWS-IAM-orange?style=for-the-badge&logo=amazon-aws)
![Cloud](https://img.shields.io/badge/Cloud-DevOps-blue?style=for-the-badge&logo=icloud)
![Beginner Project](https://img.shields.io/badge/Project-Beginner-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
# AWS-IAM-Hands-on-Lab
This project demonstrates practical understanding of AWS Identity and Access Management (IAM) by creating users, applying policies, and managing access using groups. The goal is to understand how AWS controls authentication and authorization.

🎯 Objective

To learn and implement:

IAM Users creation
IAM Policies (permissions)
IAM Groups (best practice for access management)
AWS security model (Implicit Deny & Explicit Allow)
🛠️ AWS Service Used
AWS IAM (Identity and Access Management)
Amazon S3 (for testing access permissions)
🚀 Steps Performed
1️⃣ Created IAM User (No Permissions)
Created an IAM user without attaching any policies or groups
Logged in using IAM credentials
Tried accessing Amazon S3

Result:
Access was denied ❌ due to no permissions (Implicit Deny).

2️⃣ Attached S3 Full Access Policy
Logged in as root user
Attached AmazonS3FullAccess policy to IAM user

Result:
IAM user gained access to S3 service ✔
However, no buckets were visible as none existed in the account.

3️⃣ Created IAM Group
Created an IAM group
Attached policies to the group
Added IAM users to the group

Result:
Users inherited permissions from the group ✔
This simplified access management.

🔑 Key Learnings
AWS follows Implicit Deny Model (no access unless explicitly allowed)
IAM Policies define permissions (Allow/Deny actions)
IAM Groups help manage multiple users efficiently
Best practice is to assign permissions through groups instead of individual users
IAM is used for authentication (who you are) and authorization (what you can do)
🧠 Concepts Understood
IAM User
IAM Group
IAM Policy
Permission Inheritance
AWS Security Model
