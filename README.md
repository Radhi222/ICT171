Here is the link  to my website 
https://ict171kashish.click/<br>
My Domain name is ict171kashish.click

<h1>**Pearl Threading Cloud Project**</h1>
           Pearl Threading is a beauty and self-care platform centered around professional threading and natural beauty
           treatments.Designed as a modern beauty service business, it offers a clean, comfortable environment where
           clients can receive expert threading, waxing, tinting, and henna treatments.The goal is to enhance personal
           confidence and self-expression through skilled, affordable, and culturally inspired beauty services.The core
           focus of Pearl Threading is the art of threading—an ancient, chemical-free technique of facial hair removal
           known for its precision, gentleness on skin, and ability to create clean, defined eyebrow shapes.
           This traditional method is complemented by additional services, including waxing, tinting, and henna designs to provide a 
           holistic approach to facial and skin grooming.
           <br>
<h3>**Let's start creating our website**</h3> 
---

## 🔧 EC2 Server Setup

To host the Pearl Threading website, I launched a virtual server using **Amazon EC2** (Ubuntu 22.04). The steps are listed below:

1. **Logged in** to AWS Management Console.
2. Navigated to **EC2 > Launch Instance**.
3. Selected:
   - **Ubuntu Server 22.04 LTS**
   - **t2.micro** (eligible for free tier)
4. Created a **new key pair** (e.g., `ict171keypair1-key.pem`) for SSH access.
5. Configured **Security Group rules**:
   - ✅ TCP 22 – SSH (My IP)
   - ✅ TCP 80 – HTTP (Anywhere)
6. Launched the instance and connected using this command:  
```bash
ssh -i "ict171keypair1-key.pem" ubuntu@18.214.189.146 ````


## 🌐 Installing Apache Web Server

After connecting to my EC2 instance using SSH, I installed **Apache2**, the open-source web server software.

1. **Updated package lists:**
   ```bash
   sudo apt update
