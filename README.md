https://roadmap.sh/projects/ssh-remote-server-setup
# SSH EC2 Setup with Multiple Keys and Fail2Ban

## ✅ Project Goal

Set up a remote Linux server (EC2 on AWS) and configure it to allow SSH access using **two separate SSH key pairs**. Also, install and configure **Fail2Ban** to protect against brute-force attacks.

---

## 🔧 Steps Followed

### 1. Provision EC2 Instance

- Provider: AWS EC2
- OS: Ubuntu 22.04
- Public IP: `<your-ec2-public-ip>`
- Opened port **22 (SSH)** in security group

---

### 2. SSH Key Pairs

#### Locally (WSL / Linux terminal):

```bash
ssh-keygen -t ed25519 -f ~/.ssh/aws_key1
ssh-keygen -t ed25519 -f ~/.ssh/aws_key2
# SSH EC2 Setup
