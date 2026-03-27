# 🚀 MetricFlow Ansible

![Ansible](https://img.shields.io/badge/Automation-Ansible-red?logo=ansible)
![AWS](https://img.shields.io/badge/Cloud-AWS-orange?logo=amazon-aws)
![Status](https://img.shields.io/badge/Project-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 📌 Overview
**MetricFlow Ansible** is an automated VM monitoring solution built using Ansible.  
It dynamically discovers AWS EC2 instances, collects system-level metrics, and generates a **beautiful HTML dashboard** with optional email reporting.

---

## ✨ Features

- ⚡ Dynamic AWS EC2 inventory (no static IPs)
- 🖥️ Multi-node metric collection
- 📊 CPU, Memory, Disk monitoring
- ⏱️ Uptime & Last Reboot tracking
- 🎨 HTML dashboard using Jinja2
- 📧 Email reporting system
- 🔄 Agentless architecture

---

## 🏗️ Architecture

```text
Ansible Control Node 
        ↓
AWS EC2 Instances 
        ↓
Metrics Collection 
        ↓
Aggregation 
        ↓
HTML Dashboard 
        ↓
Email Report
