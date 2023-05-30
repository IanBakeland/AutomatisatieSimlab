# Ansible Role: Create ansible.txt File

This Ansible role is used to create the `/srv/tftp/ansible.txt` file with customizable content.

## Role Tasks

The role performs the following task:

- Create the `/srv/tftp/ansible.txt` file with customizable content.

## Usage

1. Include the `ansible_file` role in your playbook.
2. Customize the content of the `ansible.txt` file by modifying the `content` parameter in the playbook.
3. Run the playbook.

Example playbook:

```yaml
---
- name: Create ansible.txt file
  hosts: your_host
  become: true

  roles:
    - ansible_file
```
Note: Make sure to replace `your_host` with the appropriate host or host group.