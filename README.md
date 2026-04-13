# Ansible Project Template

## Overview

This is my modular **Ansible Automation Project Template** built for rapid deployment, repeatability and clean structure in production environments. It follows Ansible best practices and is tailored for use in cloud automation, Linux hardening, user provisioning, service management and CI/CD integrations.

## Features

•	Modular roles/ structure
	•	Passwordless SSH control from macOS to Linux
	•	Role automation (user_provision, file_ops)
	•	GitHub execution (no CLI setup required)
	•	GitOps and CI/CD
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
