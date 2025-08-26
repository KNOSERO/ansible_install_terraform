# Ansible Install Terraform
Script for installing terraform in Ansible

## Example

```yaml
- name: Install Terraform on localhost
  hosts: localhost
  become: yes
  vars:
    arch_type: "arm64"

  tasks:
    - name: Install Terraform
      include_tasks: ./task/ansible_install_terraform/playbook.yml  
```