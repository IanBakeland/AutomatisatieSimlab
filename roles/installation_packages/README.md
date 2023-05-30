# Ansible Role: Update apt cache and install Python 3 and tftpd-hpa

This Ansible role updates the apt cache, installs Python 3, and installs tftpd-hpa. It also checks the status of the tftpd-hpa service and ensures it is started and enabled.

**Important Note:** Before running this playbook, make sure that the Squid proxy server is running in your environment.

## Role Tasks

The role performs the following tasks:

1. Update the apt cache.
2. Install Python 3.
3. Install tftpd-hpa.
4. Check the status of the tftpd-hpa service and ensure it is started and enabled.

## Usage

1. Create an Ansible playbook and include the `installation_packages` role in it.
2. Set the necessary variables, such as proxy settings if required.
3. Run the playbook.

Example playbook:

```yaml
---
- name: Update apt cache and install Python 3 and tftpd-hpa
  hosts: your_hosts
  become: true

  roles:
    - installation_packages
```
Make sure to replace `your_hosts` with the appropriate host or group of hosts where you want to perform the updates and installations.

**Note:** Ensure that the Squid proxy server is running before executing this playbook, as it may be required for accessing the necessary packages.