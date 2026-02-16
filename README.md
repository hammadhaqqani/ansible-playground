# Ansible Playground

[![Ansible Lint](https://github.com/hammadhaqqani/ansible-playground/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/hammadhaqqani/ansible-playground/actions/workflows/ansible-lint.yml)
[![GitHub Pages](https://github.com/hammadhaqqani/ansible-playground/actions/workflows/pages.yml/badge.svg)](https://hammadhaqqani.github.io/ansible-playground/)
[![Ansible](https://img.shields.io/badge/Ansible-%231A1918.svg?logo=ansible&logoColor=white)](https://www.ansible.com/)
[![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)
[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-ffdd00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/hammadhaqqani)

A collection of Ansible playbooks, roles, and examples for infrastructure automation, configuration management, and application deployment. Covers LAMP stacks, JBoss, Tomcat, MongoDB, WordPress, Windows automation, and more.

## Playbooks

| Playbook | Description |
|----------|-------------|
| **lamp_simple** | Simple LAMP stack (Apache, MySQL, PHP) deployment |
| **lamp_simple_rhel7** | LAMP stack optimized for RHEL 7 |
| **lamp_haproxy** | LAMP stack with HAProxy load balancer and Nagios monitoring |
| **jboss-standalone** | JBoss Application Server with Java app deployment |
| **tomcat-standalone** | Apache Tomcat server deployment |
| **tomcat-memcached-failover** | Tomcat with Memcached session failover and Nginx LB |
| **wordpress-nginx** | WordPress with Nginx, PHP-FPM, and MySQL |
| **wordpress-nginx_rhel7** | WordPress/Nginx stack for RHEL 7 with MariaDB |
| **mongodb** | MongoDB sharded cluster with replica sets |
| **windows** | Windows automation: IIS, users, MSI installs, PowerShell |
| **language_features** | Ansible language examples: conditionals, delegation, filters |
| **phillips_hue** | Fun: control Phillips Hue lights with Ansible |
| **rust-module-hello-world** | Custom Ansible module written in Rust |

## Project Structure

```
.
├── lamp_simple/                # Basic LAMP stack
├── lamp_simple_rhel7/          # LAMP for RHEL 7
├── lamp_haproxy/               # LAMP + HAProxy + Nagios
│   └── aws/                    # AWS-specific variant
├── jboss-standalone/           # JBoss app server
├── tomcat-standalone/          # Tomcat server
├── tomcat-memcached-failover/  # Tomcat + Memcached + Nginx
├── wordpress-nginx/            # WordPress + Nginx
├── wordpress-nginx_rhel7/      # WordPress + Nginx (RHEL 7)
├── mongodb/                    # MongoDB sharded cluster
├── windows/                    # Windows automation playbooks
│   └── wamp_haproxy/           # WAMP stack on Windows
├── language_features/          # Ansible language examples
├── phillips_hue/               # Phillips Hue integration
└── rust-module-hello-world/    # Custom Rust module
```

## Prerequisites

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/) >= 2.9
- SSH access to target hosts (Linux) or WinRM (Windows)
- Python 3.x on control node

## Quick Start

```bash
# Clone the repo
git clone https://github.com/hammadhaqqani/ansible-playground.git
cd ansible-playground

# Example: deploy a simple LAMP stack
cd lamp_simple

# Edit the hosts inventory with your server IPs
vim hosts

# Run the playbook
ansible-playbook -i hosts site.yml
```

## Usage

Each playbook directory contains:

- `site.yml` - Main playbook entry point
- `hosts` - Inventory file (edit with your server IPs)
- `group_vars/` - Variables for host groups
- `roles/` - Reusable roles with tasks, handlers, templates, and files

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Author

**Hammad Haqqani** - DevOps Architect & Cloud Engineer

- Website: [hammadhaqqani.com](https://hammadhaqqani.com)
- LinkedIn: [linkedin.com/in/haqqani](https://www.linkedin.com/in/haqqani)
- Email: phaqqani@gmail.com

---

## Support

If you find this useful, consider buying me a coffee!

[![Buy Me A Coffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/hammadhaqqani)
