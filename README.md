# ☁️ AWS Labs by Christina Leoso

Hands-on, beginner-friendly cloud security labs with clear steps, screenshots, and lessons learned.

---

## 🔐 Labs

### 1) IAM – Principle of Least Privilege
**Repo:** https://github.com/christinaleoso/aws-iam-least-privilege-lab  
**What I did:** Created two IAM users (Admin vs ReadOnly) and tested S3 actions to show how least privilege prevents misuse.  
**Receipts:** Screenshots of success vs “Access Denied”.  
**Takeaways:** Start with minimum permissions, add only what’s needed.

---

### 2) S3 – Public vs Private Buckets
**Repo:** https://github.com/christinaleoso/aws-s3-bucket-securitylab  
**What I did:** Created a private bucket, proved Access Denied, then (safely) made object public to demonstrate risk.  
**Receipts:** Before/after screenshots + browser access proof.  
**Takeaways:** Misconfigured buckets are a top breach cause—keep public access blocked by default.

---

## 📅 Roadmap (Next labs)
- CloudTrail: log & trace S3 actions
- Custom IAM policy for a single bucket path
- MFA on IAM users (and enforce with policy)

---

## 👋 About
I’m Christina Leoso, pivoting into Cloud Security. Follow my labs here and on LinkedIn.
