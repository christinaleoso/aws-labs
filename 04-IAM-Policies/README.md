# AWS Lab 04: IAM Policies

## 📌 Purpose
This lab explores **IAM policies**, how they are structured, and how they apply to users and groups in AWS.  
- Learn how policies are attached at the **user, group, or inline** level.  
- Understand how a user can inherit **multiple policies** through multiple groups.  
- Break down the **JSON structure** of an IAM policy.  

---

## 🛠️ Concepts Learned

### 1. Policy Inheritance
- Policies attached to a **group** apply to **all users** in that group.  
- A user can belong to **multiple groups**, inheriting policies from each.  
- Inline policies can be attached **directly** to a user (less common, harder to manage).  

📊 Example:  
- Developers group → Alice, Bob, Charles  
- Operations group → David, Edward  
- Audit group → Charles, David  
<img width="3672" height="1467" alt="04-IAM-Policies" src="https://github.com/user-attachments/assets/35309e58-a0c0-45bb-b05b-e2b1529d2018" />

➡️ Result:  
- Charles inherits policies from Developers + Audit.  
- David inherits policies from Operations + Audit.  

---

### 2. Policy JSON Structure
An IAM policy is written in JSON and follows this structure:

```json
{
  "Version": "2012-10-17",
  "Id": "PolicyID",
  "Statement": [
    {
      "Sid": "1",
      "Effect": "Allow",
      "Principal": { "AWS": "arn:aws:iam::123456789012:root" },
      "Action": "s3:*",
      "Resource": "arn:aws:s3:::example-bucket/*"
    }
  ]
}
