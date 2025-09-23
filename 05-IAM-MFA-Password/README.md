# AWS Lab 06: IAM MFA & Password Policy

## 📌 Purpose
This lab strengthens AWS account security by:  
- Enforcing a **strong password policy** for IAM users.
- Enabling **Multi-Factor Authentication (MFA)** on the AWS root account.  

---

## 🛠️ Steps Completed

### 1. Password Policy
- Minimum length set to 12 characters.  
- Required uppercase, lowercase, number, and special character.  
- Prevented password reuse (last 3 passwords).  
- Enabled password expiration at 90 days.  

📸 Screenshot: Password policy page.
<img width="1728" height="945" alt="05-IAM-MFA-Password" src="https://github.com/user-attachments/assets/089fd628-ac10-4446-9ad5-cb11776a121d" />
---

### 2. Enable MFA on Root Account
- Chose **virtual MFA device** (Authenticator app).  
- Scanned QR code and entered two generated codes.  
- Confirmed MFA device assignment.  

📸 Screenshot: MFA device successfully added.  
 <img width="1728" height="946" alt="05-IAM-MFA" src="https://github.com/user-attachments/assets/611af64c-8ac1-4b8e-b734-1095c00a5515" />
---

### 3. Test MFA Login
- Logged out and signed back in.  
- Entered root password → prompted for MFA code.  
- Successfully logged in with MFA.  

📸 Screenshot: Login page requiring MFA code.  
<img width="811" height="879" alt="05-IAM-MFA-Confirm" src="https://github.com/user-attachments/assets/3457d3fb-8673-4807-961d-c5f8a747e200" />

---

## ✅ Key Takeaways
- Enforcing strong password policies reduces risk of compromised credentials.  
- MFA is **critical for securing the root user**, which has full account access.  
- AWS supports up to 8 MFA devices (virtual, hardware, or security keys).  

---

## 🔗 Related Resources
- [AWS IAM Password Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_account-policy.html)  
- [Enabling MFA in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable-root.html)  
