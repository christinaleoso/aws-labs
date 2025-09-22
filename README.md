# ☁️ AWS Security Labs by Christina Leoso

Hands-on cloud security projects showing real-world risks and defenses in AWS.  
Each lab includes a step-by-step guide, screenshots, and key takeaways.

---

## 🔐 Completed Labs

### 1) IAM – Principle of Least Privilege
📂 [iam-least-privilege](./iam-least-privilege)  
**What I did:** Compared an Admin user vs. a ReadOnly user and tested S3 actions.  
**Result:** Admin succeeded, ReadOnly hit “Access Denied.”  
**Lesson:** Least privilege prevents misuse and accidents.

---

### 2) S3 – Public vs Private Buckets
📂 [s3-bucket-security](./s3-bucket-security)  
**What I did:** Created a private bucket and tested access. Then made it public to show the risk.  
**Result:** Access denied when private, world-readable when public.  
**Lesson:** Misconfigured S3 buckets are a common cause of breaches — keep Block Public Access enabled by default.

---

## 🗺️ Roadmap (Upcoming Labs)

- 🔎 **CloudTrail Logging** – Trace S3 actions in logs.  
- 🛡️ **Custom IAM Policy** – Grant object-level permissions (s3:GetObject only).  
- 🔑 **MFA on IAM Users** – Test login flows with and without MFA.  
- 🚨 **GuardDuty Alerts** – Trigger and investigate a simulated security finding.  
- 🌐 **VPC Security Groups** – Test open vs. restricted inbound rules.  

---

## 👩‍💻 About Me
I’m Christina Leoso, pivoting into Cloud Security.  
These labs are part of my journey to build hands-on skills and share what I’m learning with others.  

📌 Connect with me on LinkedIn: [linkedin.com/in/christinaleoso](https://linkedin.com/in/christinaleoso)
