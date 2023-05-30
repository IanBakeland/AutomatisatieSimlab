# Ansible Role: Update and Configure tftpd-hpa

This Ansible role updates the tftpd-hpa configuration by removing the old configuration and updating it with a new one. It also restarts the tftpd-hpa service.

## Role Tasks

The role performs the following tasks:

1. Remove the old tftpd-hpa configuration.
2. Update the /etc/default/tftpd-hpa file with the new configuration.
3. Restart the tftpd-hpa service.

## Usage

1. Include the `tftpd_config` role in your playbook.
2. Run the playbook.

Example playbook:

```yaml
---
- name: Update and Configure tftpd-hpa
  hosts: your_host
  become: true

  roles:
    - tftpd_config
```