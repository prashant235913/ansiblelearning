# Deploying and Configuring Web Server on AWS EC2 with Ansible

## Overview
This project demonstrates the deployment and configuration of a web server on AWS EC2 instances using Ansible. It automates the setup process, from server provisioning to deploying a success page.
![](https://miro.medium.com/v2/resize:fit:1400/1*LaozQKQr0RP0-r9A4brC3w.png)
## Table of Contents
- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [How to Use](#how-to-use)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites
Make sure you have the following installed:
- [Ansible](https://www.ansible.com/)
- [AWS CLI](https://aws.amazon.com/cli/)
- AWS EC2 instances with SSH access


## PROJECT STRUCTURE
```plaintext
.
├── inventory.ini
├── playbooks
│   └── main.yml
├── roles
│   └── software
│       ├── handlers
│       │   └── main.yml
│       └── tasks
│           └── main.yml
└── success.html
```

- `inventory.ini`: Defines the hosts (EC2 instances).
- `playbooks/main.yml`: Main playbook for deploying and configuring the web server.
- `roles/software`: Ansible role containing tasks and handlers.

## How to Use
1. Clone the repository: `git clone [repo-url]`
2. Configure your AWS credentials using the AWS CLI.
3. Update the `inventory.ini` file with your EC2 instance details.
4. Run the Ansible playbook: `ansible-playbook -i inventory.ini playbooks/main.yml`

## Troubleshooting
If you encounter issues, check the following:
- Ensure Ansible and AWS CLI are installed.
- Verify AWS credentials and EC2 instance accessibility.
- Review Ansible playbook logs for detailed information.

