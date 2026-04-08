# ☁️ AWS Cloud Homelab

A personal cloud homelab built on AWS, documenting the end-to-end process of provisioning, configuring, and managing a Linux-based virtual server from scratch. This repo serves as a living reference for cloud infrastructure, Linux administration, and web server deployment skills.

---

## 🗺️ Project Overview

| Module | Description | Status |
|---|---|---|
| EC2 Instance Setup | Launch and configure an Ubuntu EC2 instance | ✅ Complete |
| SSH Access | Connect to the instance via OpenSSH | ✅ Complete |
| Network Security | Configure VPC, security groups, and inbound rules | ✅ Complete |
| Apache Web Server | Install and verify Apache2 on Ubuntu | ✅ Complete |
| Linux Administration | User management, package management, system commands | ✅ Complete |

---

## ⚙️ Module Details

### 1. EC2 Instance Setup

- Created an AWS account and navigated to the EC2 Management Console
- Launched an Ubuntu 24.04.4 LTS EC2 instance
- Configured a key pair for SSH authentication
- Set network and subnet settings within a custom VPC

### 2. SSH Access

- Connected to the instance via SSH using the generated key pair
- Also tested access via EC2 Instance Connect using the public IP

```bash
ssh -i "your-key.pem" ubuntu@<public-ip>
```

### 3. Network Security

- Configured AWS Security Group inbound rules to control traffic
- Restricted access by port and source IP
- Validated firewall rules using EC2 security group settings

### 4. Apache Web Server Installation

- Updated system packages and installed Apache2 on the Ubuntu instance
- Verified installation via terminal output and systemd service status

```bash
sudo apt update
sudo apt install apache2 -y
```

- Confirmed Apache2 v2.4.58 installed with systemd service enabled
- Verified no post-install restarts required

### 5. Linux Administration

- Created and managed Linux user accounts
- Practiced package management with APT
- Navigated the Linux filesystem and used core CLI commands

---

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| AWS EC2 | Virtual server provisioning |
| AWS VPC | Network configuration and isolation |
| AWS Management Console | Cloud resource management |
| Ubuntu Server 24.04 LTS | Linux operating system |
| Apache2 | Web server |
| OpenSSH | Remote server access |
| APT | Package management |

---

## 🧠 Skills Demonstrated

- Cloud infrastructure provisioning on AWS
- EC2 instance launch, configuration, and management
- Network security configuration (VPC, security groups, inbound rules)
- Remote server administration via SSH
- Web server deployment and verification
- Linux system administration and CLI navigation
- APT package management on Ubuntu

---

## ⚠️ Note

This homelab is built for learning and documentation purposes. New modules will be added as the environment expands.# Creating an AWS Homelab
