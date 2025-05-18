# SSH EC2 Setup with Fail2Ban

This project documents the steps taken to set up a remote Linux EC2 server on AWS with SSH access configured via two key pairs, and an optional Fail2Ban installation.

---

## ✅ Objectives

- Setup a remote EC2 Ubuntu server.
- Create and add two new SSH key pairs.
- Configure local `~/.ssh/config` to allow connections using aliases.
- Test SSH connection using both keys.
- Stretch Goal: Install and configure Fail2Ban.

---

## 🔐 SSH Key Generation

```bash
ssh-keygen -t rsa -f ~/.ssh/aws_key1
ssh-keygen -t rsa -f ~/.ssh/aws_key2

