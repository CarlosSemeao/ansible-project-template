# Ansible Project Template

## Overview

This is my modular **Ansible Automation Project Template**, built for rapid deployment, repeatability, and clean structure in production-like environments. It follows Ansible best practices, GitOps-ready principles, and is tailored for use in cloud automation, Linux hardening, user provisioning, service management, and CI/CD integrations.

This repository is not just a folder layout — it’s a **battle-tested framework** I use in real automation labs and will scale with future roles, playbooks, and Ansible Galaxy roles.

## Features

•	Modular roles/ structure
	•	Passwordless SSH control from macOS to Linux
	•	Role-based automation (user_provision, file_ops)
	•	Click-by-click GitHub execution (no CLI setup required)
	•	GitOps-compatible and CI/CD-ready
	•	Easily extendable for:
	•	Cloud provisioning (AWS, Azure)
	•	Linux hardening and user management
	•	Service deployment
	•	Cron jobs / scheduled ops
	•	Compliance automation

## Directory Structure

```bash
ansible-project-template/
├── ansible.cfg               # Ansible configuration
├── inventories/
│   └── hosts.ini             # Inventory file
├── playbooks/
│   └── main.yml              # Main playbook (calls roles)
├── roles/
│   ├── user_provision/       # Creates the devops_user on remote machine
│   │   ├── tasks/
│   │   │   └── main.yml
│   │   └── vars/
│   │       └── main.yml
│   └── file_ops/             # Manages /opt/ops.txt with date/time stamp
│       └── tasks/
│           └── main.yml
├── .gitignore
└── README.md
```
