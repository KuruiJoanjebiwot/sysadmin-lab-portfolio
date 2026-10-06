# Enterprise Hybrid Infrastructure & Systems Engineering Lab

##  Architectural Overview
This repository contains production-ready Infrastructure-as-Code (IaC), Active Directory configuration scripts, containerized web service stacks, and Zabbix monitoring setups simulating a hybrid enterprise IT environment.

### Network Topology & Hosts
* **Active Directory DC (`win-dc01`):** `192.168.10.10` (Windows Server 2022)
* **Linux Infrastructure Node (`ubuntu-node01`):** `192.168.10.20` (Ubuntu 22.04 LTS)
* **Subnet:** `192.168.10.0/24`

---

## 🛠 Features & Capabilities

### 1. Active Directory & Identity Management
* Provisioned AD DS Forest (`corp.local`) and core DNS resolution services.
* Automated Remote Server Administration Tools (RSAT) deployment across management nodes using Ansible.

### 2. Configuration Management & Automation (Ansible)
* Executed baseline system patching, security updates, and core package management via `/ansible/site.yml`.
* Implemented multi-OS playbooks targeting both Debian/Ubuntu and Windows endpoints.

### 3. Microservices & Web Application Hosting (Docker)
* Deployed containerized Nginx web server mounted with custom web assets (`/docker/docker-compose.yml`).
* Integrated containerized Zabbix Agent 2 sidecars for real-time application metrics collection.

### 4. Infrastructure Health Monitoring (Zabbix Stack)
* Deployed multi-container Zabbix 6.4 LTS stack with MySQL database backend and Nginx frontend web console (`/zabbix/docker-compose.yml`).
* Configured real-time metric tracking for CPU load, RAM usage, disk I/O, and service health across hosts.

---

##  Proof of Work & Verification
