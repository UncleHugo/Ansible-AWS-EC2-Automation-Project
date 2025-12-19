# Ansible-AWS-EC2-Automation-Project

This project demonstrates production-style infrastructure automation on AWS using Ansible. It focuses on repeatable provisioning, secure access configuration, and conditional operations based on operating system facts.

The goal is not just to create instances, but to show clean automation patterns a DevOps engineer would actually use.

### Key Capabilities Demonstrated

- Infrastructure provisioning on AWS using Ansible

- Scalable resource creation using loops

- Secure, passwordless SSH authentication

- OS-aware automation using gathered facts

- Idempotent and modular playbook design

### Architecture Overview

*_Control Node_*: Ansible (runs locally using connection: local)

Cloud Provider: AWS EC2

*_Managed Nodes_*:

2 × Ubuntu EC2 instances

1 × AWS Linux EC2 instance

All infrastructure is provisioned and managed via code.
