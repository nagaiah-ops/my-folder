# 🚀 DevOps Learning Path: Linux, Shell Scripting, Ansible & Terraform



Welcome to your structured DevOps learning repository. This guide takes you from operating system fundamentals to automated infrastructure management and configuration.

---

## 📁 Repository Structure

```text
├── 01-linux/
│   ├── notes/
│   ├── practice-commands/
│   └── scripts/
├── 02-shell-scripting/
│   ├── basics/
│   ├── projects/
│   └── solutions/
├── 03-ansible/
│   ├── inventories/
│   ├── playbooks/
│   └── roles/
└── 04-terraform/
    ├── main.tf
    ├── variables.tf
    └── outputs.tf
```

---

## 🛠️ Curriculum Overview

### 1. 🐧 Linux (The Backbone of DevOps)
Learn how to navigate, manage, and troubleshoot Linux environments where most cloud workloads and containers run.

* **Core Topics:**
  * File system hierarchy (`/etc`, `/var`, `/usr`, `/home`)
  * Basic & intermediate CLI commands (`ls`, `grep`, `awk`, `sed`, `find`, `top`, `htop`, `netstat`)
  * File permissions and ownership (`chmod`, `chown`, `umask`)
  * User and group management (`useradd`, `passwd`, `sudoers`)
  * Process management and service controls (`systemctl`, `journalctl`, `ps`, `kill`)
  * Networking & SSH configuration (`scp`, `ssh-keygen`, `iptables`, basic `firewalld`)
* **Hands-on Exercise:**
  * Write a script that checks disk usage (`df -h`) and sends a warning log if usage exceeds 80%.

---

### 2. ⚙️ Shell Scripting (Bash)
Automate repetitive system administration tasks and build custom helper scripts.

* **Core Topics:**
  * Bash syntax, shebang (`#!/bin/bash`), and execution modes
  * Variables, data types, and user input (`read`)
  * Conditional statements (`if/else`, `case`) and loops (`for`, `while`, `until`)
  * Functions, arguments (`$1`, `$2`, `$@`), and exit codes (`$?`)
  * Error handling and debugging (`set -e`, `set -u`, `bash -x`)
* **Hands-on Exercise:**
  * Create a backup script that compresses a target directory into a timestamped `.tar.gz` file and deletes backups older than 7 days.

---

### 3. 🤖 Ansible (Configuration Management & Automation)
Manage software installations, server configurations, and application deployments across multiple nodes without agent overhead.

* **Core Topics:**
  * Architecture (Control Node vs. Managed Nodes) & SSH-based communication
  * Static & dynamic inventory files (`hosts.ini` / `hosts.yml`)
  * Ad-hoc commands vs. Playbooks (YAML syntax)
  * Writing reusable Tasks, Handlers, and Variables
  * Ansible Roles and Galaxy structure
  * Idempotency in automation
* **Hands-on Exercise:**
  * Write a playbook that updates apt cache, installs `nginx`, copies a custom `index.html` file, and ensures the service is running and enabled on 2 remote virtual machines.

---

### 4. ☁️ Terraform (Infrastructure as Code - IaC)
Provision and manage cloud or on-premise infrastructure declaratively.

* **Core Topics:**
  * What is IaC? Declarative vs. Imperative models
  * Terraform workflow (`init`, `plan`, `apply`, `destroy`)
  * Core HCL (HashiCorp Configuration Language) syntax:
    * Providers (`aws`, `azure`, `local`, etc.)
    * Resources and Data Sources
    * Variables (`variables.tf`), Outputs (`outputs.tf`), and `terraform.tfvars`
  * State management (`terraform.tfstate`, remote state in S3/DynamoDB, and state locking)
  * Modules for code reusability
* **Hands-on Exercise:**
  * Write a Terraform configuration to provision a Virtual Private Cloud (VPC), a security group allowing SSH/HTTP, and an EC2 instance.

---

## 📚 Recommended Resources & References
* **Roadmaps:** Explore structured paths like the [DevOps Roadmap](https://github.com/milanm/DevOps-Roadmap) and community hubs like [Into The DevOps](https://github.com/NotHarshhaa/into-the-devops/blob/master/README.md).
* **Documentation:**
  * [Linux man pages / TLDR pages](https://tldr.sh)
  * [Ansible Official Documentation](https://ansible.com)
  * [Terraform Registry & Docs](https://hashicorp.com)

---

## 🎯 Suggested Learning Schedule (4 Weeks)
* **Week 1:** Master Linux CLI, file permissions, and basic networking.
* **Week 2:** Practice Bash scripting by writing 5 automation scripts.
* **Week 3:** Build Ansible playbooks and configure local/cloud test servers.
* **Week 4:** Write Terraform code to spin up and tear down cloud infrastructure.
