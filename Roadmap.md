```markdown
# 🎯 Cloud & DevOps - Basic Roadmap for Beginners

> **Target:** Entry Level Cloud/DevOps Job & Internship  
> **Duration:** 3-4 Months  
> **Level:** Beginner to Basic  

---

## 📋 Table of Contents

- [Step 1: Linux](#step-1-linux-strong-karo)
- [Step 2: Git & GitHub](#step-2-git--github-seekho)
- [Step 3: AWS Cloud Basics](#step-3-aws-cloud-basics)
- [Step 4: Docker Basics](#step-4-docker-basics)
- [Step 5: Projects](#step-5-basic-project-banao)
- [Monthly Plan](#-month-by-month-plan)
- [Resources](#-free-resources)
- [Daily Routine](#-daily-routine)

---

## 📌 Step 1: Linux Strong Karo
⏱️ **Time: 2-3 Weeks**

### Basic Commands
```bash
# File Commands
ls, cd, pwd, mkdir, rm, cp, mv

# File Permission
chmod 755 file.txt
chown user file.txt

# User Management
useradd username
passwd username

# Process Commands
ps aux
top
kill <process_id>

# Networking Commands
ping google.com
ifconfig
netstat
ssh user@ip_address

# Package Install
sudo apt update
sudo apt install nginx
```

### Shell Scripting (Basic)
```bash
#!/bin/bash

echo "Hello World"
name="Rahul"
echo "My name is $name"

# If condition
if [ $name == "Rahul" ]
then
  echo "Name is correct"
fi
```

### 🛠️ Practice Tasks
- [ ] VirtualBox download karo (Free)
- [ ] Ubuntu install karo
- [ ] Daily 1 hour practice karo
- [ ] 5 simple shell scripts banao

---

## 📌 Step 2: Git & GitHub Seekho
⏱️ **Time: 1 Week**

### Basic Git Commands
```bash
git init              # New repo start karo
git add .             # Files add karo
git commit -m "msg"   # Save karo
git push origin main  # GitHub pe upload karo
git pull              # Download latest code
git clone <url>       # Kisi ka code download karo
git status            # Current status dekho
git log               # History dekho
```

### 🛠️ Practice Tasks
- [ ] GitHub account banao (Free)
- [ ] Apna first repository banao
- [ ] Code push karo
- [ ] Profile achha banao
      (Recruiters GitHub dekhte hain)

---

## 📌 Step 3: AWS Cloud Basics
⏱️ **Time: 4-5 Weeks**

### Pehle FREE Account Banao
```
👉 aws.amazon.com/free
✅ 12 months free services milti hain
✅ Credit card chahiye (Charge nahi hoga free tier mein)
```

### Sirf Ye 5 Services Seekho

#### 1️⃣ IAM - Users & Permissions
```
- AWS account me users banao
- Permissions dena seekho
- Root account mat use karo
- Access Key banana seekho
```

#### 2️⃣ EC2 - Virtual Server
```
- Server launch karna seekho
- SSH se connect karna seekho
- Server start/stop karna
- Security Groups (Firewall)
```

#### 3️⃣ S3 - Storage Service
```
- Bucket banana
- Files upload karna
- Static website host karna
- Public/Private access
```

#### 4️⃣ VPC - Networking
```
- Virtual Private Cloud kya hai
- Subnets kya hoti hain
- Internet Gateway kya hai
```

#### 5️⃣ CloudWatch - Monitoring
```
- Server ki health dekhna
- Alerts set karna
- Logs dekhna
```

### 🛠️ Practice Tasks
- [ ] Task 1: EC2 server launch karo
- [ ] Task 2: SSH se server connect karo
- [ ] Task 3: Nginx install karo server pe
- [ ] Task 4: S3 me website host karo
- [ ] Task 5: IAM user banao

---

## 📌 Step 4: Docker Basics
⏱️ **Time: 2-3 Weeks**

### Docker Kya Hai?
```
Normal:  Har computer pe alag setup karna padta hai
Docker:  Ek baar setup karo, kahin bhi chalaao

Jaise ek tiffin box hai jo khana
safe rakhta hai aur kahin bhi le ja sako
```

### Basic Docker Commands
```bash
# Docker Install karo (Ubuntu pe)
sudo apt install docker.io

# Basic Commands
docker --version          # Version check
docker pull nginx         # Image download
docker images             # Images list
docker run nginx          # Container start
docker ps                 # Running containers
docker stop <id>          # Container stop
docker rm <id>            # Container delete
```

### Dockerfile Example
```dockerfile
FROM ubuntu                                    # Base image
RUN apt-get update                             # Update karo
RUN apt-get install -y nginx                   # Nginx install

COPY index.html /var/www/html/                 # File copy karo

EXPOSE 80                                      # Port open karo

CMD ["nginx", "-g", "daemon off;"]             # Start command
```

### 🛠️ Practice Tasks
- [ ] Task 1: Docker install karo
- [ ] Task 2: Nginx container chalaao
- [ ] Task 3: Simple Dockerfile banao
- [ ] Task 4: Docker Hub pe account banao
- [ ] Task 5: Apna image push karo Docker Hub pe

---

## 📌 Step 5: Basic Project Banao
⏱️ **Time: 2 Weeks**

### 🔹 Project 1: Simple Website on AWS S3
```
Kya karoge:
✅ HTML website banao
✅ S3 pe upload karo
✅ Public access do
✅ Website live ho jayegi

Kya seekhoge:
- AWS S3
- Static website hosting
- Public access settings
```

### 🔹 Project 2: EC2 pe Website Deploy
```
Kya karoge:
✅ EC2 server launch karo
✅ SSH se connect karo
✅ Nginx install karo
✅ Website files daalo
✅ Website live ho jayegi

Kya seekhoge:
- EC2 practical knowledge
- Linux commands
- Nginx web server
- SSH connection
```

### 🔹 Project 3: Docker Container
```
Kya karoge:
✅ Simple web app banao
✅ Dockerfile banao
✅ Image build karo
✅ Container run karo
✅ Docker Hub pe push karo

Kya seekhoge:
- Docker practical
- Containerization concept
- Docker Hub use
```

---

## 📅 Month by Month Plan

| Month | Week | Topic |
|-------|------|-------|
| Month 1 | Week 1-2 | Linux Practice |
| Month 1 | Week 3 | Git & GitHub |
| Month 1 | Week 4 | AWS Account + IAM + EC2 |
| Month 2 | Week 1-2 | AWS (S3, VPC, CloudWatch) |
| Month 2 | Week 3-4 | Docker Basics |
| Month 3 | Week 1-2 | Projects Banao |
| Month 3 | Week 3 | Resume Banao |
| Month 3 | Week 4 | Job Apply Karna Shuru Karo |

---

## 📚 Free Resources

### YouTube Channels
| Channel | Language | Topic |
|---------|----------|-------|
| Abhishek Veeramalla | Hindi | DevOps (Best) |
| Shubham Londhe | Hindi | Cloud & DevOps |
| TechWorld with Nana | English | Docker & K8s |

### Websites
| Website | Use |
|---------|-----|
| [AWS Skill Builder](https://skillbuilder.aws) | Free AWS Learning |
| [KodeKloud](https://kodekloud.com) | Free Labs |
| [Play with Docker](https://labs.play-with-docker.com) | Free Docker Practice |
| [AWS Free Tier](https://aws.amazon.com/free) | Free AWS Practice |

---

## ⚡ Daily Routine

```
🕐 2-3 Hours Daily Enough Hai

1 Hour   → Video dekhna + Theory
1 Hour   → Hands-on Practice
30 Min   → Notes likhna
30 Min   → LinkedIn active rehna
```

---

## ✅ Important Tips

```
1. Theory kam, Practice zyada karo
2. Har cheez GitHub pe daalo
3. LinkedIn profile banao
4. Ek step complete karo phir aage badho
5. Confusion me mat raho - basics pakke karo
6. Daily consistency sabse important hai
```

---

## 🎯 Entry Level Job ke liye Minimum Skills

| Skill | Level |
|-------|-------|
| Linux | Good Knowledge |
| Git/GitHub | Must Have |
| AWS Basics (EC2, S3, IAM) | Basic |
| Docker | Basic |
| Projects | 2-3 Projects on GitHub |
| Resume | Well Written |
| LinkedIn | Active Profile |

---

## 🏢 Job Apply Karo Yahan

### Job Portals
- [LinkedIn](https://linkedin.com)
- [Naukri.com](https://naukri.com)
- [Internshala](https://internshala.com)
- [Indeed](https://indeed.com)

### Job Titles Search Karo
```
- Junior DevOps Engineer
- Cloud Support Engineer
- AWS Cloud Engineer Fresher
- DevOps Intern
- Cloud Operations Engineer
- Linux System Administrator
```

---

<div align="center">

### 💪 Consistency is the Key to Success!

**Made with ❤️ for BCA Freshers**

</div>
```

---

## 📁 Ise Kaise Use Karo?

```bash
# Step 1: GitHub pe new repository banao
# Repository name: cloud-devops-roadmap

# Step 2: README.md file banao
# Upar diya hua content copy karo

# Step 3: Commit karo
git add README.md
git commit -m "Added Cloud DevOps Roadmap"
git push origin main
```

---

> 💡 **Tip:** Yeh README.md aapke
> GitHub profile pe bahut achha lagega
> aur recruiters ko impress karega! 🚀
