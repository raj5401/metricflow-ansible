# MetricFlow Ansible

## Overview
MetricFlow Ansible is an automated VM monitoring solution built using Ansible. It dynamically discovers AWS EC2 instances, collects system-level metrics, and generates a consolidated HTML dashboard with optional email reporting.

## Features
- Dynamic AWS EC2 inventory (no static IPs)
- Multi-node metric collection
- CPU, Memory, Disk usage monitoring
- Uptime and last reboot tracking
- Clean HTML dashboard using Jinja2 templates
- Email-based reporting system
- Scalable and agentless architecture

## Architecture
Ansible Control Node → AWS EC2 Instances → Metrics Collection → Aggregation → HTML Report → Email Delivery

## Tech Stack
- Ansible
- AWS EC2
- Python (boto3)
- Jinja2 (templating)

## How It Works
1. Ansible dynamically fetches EC2 instances using AWS tags
2. Metrics are collected from all nodes in parallel
3. Data is aggregated on the control node
4. HTML report is generated using Jinja2
5. Report is optionally sent via email

## Run the Project

```bash
cd vm-monitor
ansible-playbook -i inventory/aws_ec2.yml playbooks/main.yml
