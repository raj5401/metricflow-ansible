# 🚀 MetricFlow Ansible

![Ansible](https://img.shields.io/badge/Automation-Ansible-red?logo=ansible)
![AWS](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazon-aws)
![Status](https://img.shields.io/badge/Project-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 📌 Overview
**MetricFlow Ansible** is a modular, role-based VM monitoring system built using Ansible.  
It dynamically discovers AWS EC2 instances, collects system-level metrics, and generates a **centralized HTML dashboard with automated email reporting**.

---

## ✨ Features

- ⚡ Dynamic AWS EC2 inventory (no static IPs)
- 🖥️ Parallel multi-node metric collection
- 📊 CPU, Memory, Disk usage monitoring
- ⏱️ Uptime & Last Reboot tracking
- 🧩 Modular **Ansible role-based architecture**
- 🎨 HTML dashboard using Jinja2 templates
- 📧 Automated email reporting
- 🔄 Agentless and idempotent execution

---

## 🏗️ Architecture

```text
Ansible Control Node
        ↓
Dynamic AWS EC2 Inventory
        ↓
Ansible Roles
   ├── Metrics Collection
   ├── Report Generation
   └── Email Notification
        ↓
HTML Dashboard
        ↓
Email Delivery
