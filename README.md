# Ansible Playbook: Installation and Configuration of TFTP

This Ansible playbook is used to install and configure TFTP (Trivial File Transfer Protocol) on the target hosts.

## Playbook Tasks

The playbook performs the following tasks:

1. Install the necessary packages.
2. Configure the TFTP server.
3. Create the `ansible.txt` file via Ansible.

## Usage

1. Define your inventory file with the target hosts under the group `myhosts`.
2. Customize the playbook according to your requirements (e.g., update package names, TFTP configuration, content of the `ansible.txt` file).
3. Run the playbook using the following command:

   ```shell
   ansible-playbook tftp.yml
   ```
Before running this playbook, ensure that you have the necessary access to the target hosts and that the required packages and services are available in your package repositories.

Make sure to review and adjust the configurations within the roles (`tftpd_config`, `ansible_file`) to suit your environment and specific requirements.