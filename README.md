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
ssh -i "ict171keypair1-key.pem" ubuntu@18.214.189.146
```

   ## 🌐 Installing Apache Web Server

After connecting to my EC2 instance using SSH, I installed **Apache2**, the open-source web server software.

1. **Updated package lists:**

    ```bash
    sudo apt update
    ```

2. **Installed Apache2:**

    ```bash
    sudo apt install apache2
    ```

3. **Tested Apache by visiting:**

    ```
    http://18.214.189.146 or http://ict171kashish.click
    ```

If Apache is working, the browser shows the default Apache2 Ubuntu welcome page.

---

## 🖥️ Creating the Website with HTML & CSS

After confirming Apache was working, I created a simple custom website for **Pearl Threading** by editing the default Apache landing page.

1. **Opened the index.html file using nano:**

    ```bash
    sudo nano /var/www/html/index.html
    ```

2. **Wrote all my HTML and CSS manually inside this file.**  
   I included:
   - A homepage introducing Pearl Threading services
   - Service descriptions (e.g., eyebrow threading, facial threading, etc.)
   - Basic CSS styling using `<style>` tags within the same HTML file

3. **Saved and exited the file** by pressing `Ctrl + O`, `Enter`, then `Ctrl + X`.

4. **Tested the website** in my browser by visiting:

    ```
    http://18.214.189.146 or http://ict171kashish.click
    ```

The website successfully displayed my custom Pearl Threading homepage with all the content and styling I wrote inside `index.html`.


## 🖼️ Website Screenshot

Here is a screenshot of my Html and css code 

![Homepage Screenshot](web1.PNG)

![Homepage Screenshot](web2.PNG)





