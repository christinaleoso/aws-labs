# AWS Lab 01: IAM Users & Groups

## 📌 Purpose
The purpose of this lab is to practice **Identity and Access Management (IAM)** in AWS.  
- Avoid using the **root account** for daily operations.  
- Create **IAM users** and place them in **groups** to manage permissions more securely.  
- Understand that IAM is a **global service** (not region-specific).  

---

## 🛠️ Steps Completed

### 1. Open IAM Dashboard
- Navigated to the IAM console from the AWS Management Console.  
- Observed that IAM is global (no region selection).  

📸 Screenshot:  
<img width="1728" height="940" alt="iam-dashboard" src="https://github.com/user-attachments/assets/10094d47-6ff7-4d43-a34d-de2c043a2580" />

---

### 2. Create IAM User
- Created a user (e.g., `AdminUser`).  
- Enabled AWS Management Console access.  
- Set a custom password for login.  

📸 Screenshot:  
<img width="1728" height="1117" alt="create-user" src="https://github.com/user-attachments/assets/aea1433b-e978-4e59-a711-0d99f3640deb" />

---

### 3. Create IAM Group
- Created a group named **`Admins`**.  
- Attached the **AdministratorAccess** managed policy.  

📸 Screenshot:  
<img width="1728" height="963" alt="create-group" src="https://github.com/user-attachments/assets/eac24944-c5b3-4b20-bd5a-faacf4d6a278" />

---

### 4. Add User to Group
- Added `AdminUser` to the `Admins` group.  
- Verified that the user inherits **AdministratorAccess** via the group.  

📸 Screenshot:  
<img width="1728" height="944" alt="user-in-group" src="https://github.com/user-attachments/assets/73a41aef-7ff7-4c67-9fb8-e26bdeddf319" />

---

### 5. Verify User & Group
- Viewed **Group Details** showing attached AdministratorAccess policy.  

📸 Screenshots:  
<img width="1728" height="942" alt="group-details" src="https://github.com/user-attachments/assets/3c2ef33c-d365-4691-ac17-f0fbb2e8eaad" />

---

### 6. Create Account Alias
- Created an **account alias** to simplify login URLs.  

📸 Screenshot:  
<img width="1728" height="1117" alt="account-alias" src="https://github.com/user-attachments/assets/e4162a09-142d-4c46-907a-fe850e21d3c1" />

---

### 7. Test IAM Login
- Opened a private browser window.  
- Logged in as `AdminUser` using the alias URL.  
- Compared **Root login** (left window) vs **IAM User login** (private window).  

📸 Screenshot:  
<img width="1728" height="1115" alt="iam-vs-root-login" src="https://github.com/user-attachments/assets/6eaecb77-afb3-4859-9d00-6605c0e339ad" />)

---

## ✅ Key Takeaways
- IAM is a **global service**.  
- Best practice = **do not use the root account** for daily tasks.  
- Users inherit permissions from **groups** → easier to manage.  
- Custom **account aliases** simplify sign-in for IAM users.  

---

## 🔗 Related Resources
- [AWS IAM Documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)  
- [AWS Security Best Practices](https://aws.amazon.com/iam/resources/best-practices/)  

