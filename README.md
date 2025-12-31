# Ansible-AWS-EC2-Automation-Project

This project demonstrates production-style infrastructure automation on AWS using Ansible. It focuses on repeatable provisioning, secure access configuration, and conditional operations based on operating system facts.

The goal is not just to create instances, but to show clean automation patterns a Cloud engineer would actually use.

### Key Capabilities Demonstrated

- Infrastructure provisioning on AWS using Ansible

- Scalable resource creation using loops

- OS-aware automation using gathered facts

- Idempotent and modular playbook design

### Architecture Overview

*_Control Node_*: Ansible (runs locally using connection: local)

Cloud Provider: AWS EC2

*_Managed Nodes_*:

2 × Ubuntu EC2 instances

1 × AWS Linux EC2 instance

All infrastructure is provisioned and managed via code.


## Task : EC2 Provisioning with Ansible Loops

Ansible is used to provision three EC2 instances in AWS using a single playbook and loop logic:

Two Ubuntu instances

One AWS Linux instance

#### Why this matters:

- Avoids duplicated YAML

- Scales cleanly as instance count grows

- Mirrors how infrastructure is defined in real DevOps workflows

The playbook executes locally on the control node and interacts directly with AWS APIs.


### Prerequisites

1. Ansible installed on the control node

2. AWS account with EC2 permissions

3. AWS credentials configured (env vars or AWS config)

4. Required Ansible AWS collections installed

5. SSH key pair available

### Execution Flow

1. Provision EC2 instances on AWS


