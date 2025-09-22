# 🔐 AWS S3 Bucket Security Lab: Public vs. Private

## 📌 Project Overview
This project demonstrates why **S3 bucket permissions matter** and how the **principle of least privilege** applies to cloud storage.  

I created an S3 bucket, uploaded a test file, and showed the difference between **private access (secure)** and **public access (misconfigured)**.  

---

## 🛠️ Tools & Services
- AWS Free Tier  
- Amazon S3 (Simple Storage Service)  

---

## 📂 Steps Taken

### 1. Created a Private Bucket
- Created `private-bucket-43211` with **Block Public Access ON**.  
- Uploaded `hello.txt` with the text:  
- Tried accessing the file URL → Got **Access Denied**.  

📸 *Screenshot: S3 console showing bucket with “Block Public Access = On”*  
<img width="1704" height="939" alt="bucket-private" src="https://github.com/user-attachments/assets/ed4ebc67-2b2f-44ce-8be0-fc8ec196bdbe" />
📸 *Screenshot: Browser showing Access Denied error*  
<img width="1728" height="966" alt="access-denied" src="https://github.com/user-attachments/assets/7ea6fde9-7a92-46d0-ba7b-e559687fb952" />

---

### 2. Made the Bucket/Object Public
- Disabled **Block Public Access** at the bucket level.  
- Updated the object’s **ACL (Access Control List)** to allow **Read access for Everyone**.  
- Accessed the file URL → Successfully displayed file content.  

📸 *Screenshot: Browser showing the file text*  
<img width="1728" height="975" alt="bucket-public" src="https://github.com/user-attachments/assets/d4364966-243f-454e-a240-934cf4908676" />

---

### 3. Cleanup
- Removed object-level public access.  
- Deleted the `hello.txt` file.  
- Deleted the test bucket.  

---

## 🎯 Key Takeaways
- **Private bucket (default):** Protects files from unauthorized access.  
- **Public bucket (misconfigured):** Anyone on the internet can read your files.  
- Misconfigured S3 buckets are one of the **most common causes of cloud breaches**.  

---

## 🚀 Next Steps
- Explore **bucket policies** for more granular control.  
- Test CloudTrail logs to monitor access attempts.  
- Apply the **principle of least privilege** by default: deny all, allow only what’s needed.

