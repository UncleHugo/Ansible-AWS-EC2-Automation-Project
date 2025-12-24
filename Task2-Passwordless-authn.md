### TASK 2

Passwordless SSH authentication is configured between the Ansible control node and all EC2 instances.
This allows Ansible to connect and execute playbooks securely without requiring manual password entry, enabling fully automated provisioning and configuration.

Public key authentication is used to ensure secure, consistent, and repeatable access across all managed nodes.

_ssh-copy-id -f "-o IdentityFile <PATH TO PEM FILE>" ubuntu@INSTANCE-PUBLIC-IP_


