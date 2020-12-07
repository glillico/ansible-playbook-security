# Role Name

A ansible playbook that run a number of roles that together perform some basic server hardening.

## Requirements

All roles listed in requirements.yml must be present.

### Installation

- Clone this repository.
    - `$ git clone https://github.com/glillico/ansible-playbook-security.git`
  - Change to the git repositories directory.
    - `cd ansible-playbook-security`
  - Install the role requirements.
    - ~~`$ ansible-galaxy install -r requirements.yml`~~
    - git clone https://github.com/glillico/ansible-role-firewall roles/ansible-role-firewall
    - git clone https://github.com/glillico/ansible-role-configure_sshd roles/ansible-role-configure_sshd
    - git clone https://github.com/glillico/ansible-role-copy_etc_issue roles/ansible-role-copy_etc_issue 
    - git clone https://github.com/glillico/ansible-role-configure_sudo roles/ansible-role-configure_sudo
    - git clone https://github.com/glillico/ansible-role-set_hostname roles/ansible-role-set_hostname
    - git clone https://github.com/glillico/ansible-role-update_pkgs roles/ansible-role-update_pkgs
    - git clone https://github.com/glillico/ansible-role-auto_pkg_updates roles/ansible-role-auto_pkg_updates
    - git clone https://github.com/glillico/ansible-role-setup_users roles/ansible-role-setup_users
  - Run the below command to run the playbook, you will need to enter your account password when prompted.
    - `$ ansible-playbook -i inventory site.yml -Kb`

## Role Variables

See the individual roles for variable descriptions.

- [ansible-role-firewall](https://github.com/glillico/ansible-role-firewall)<br>
- [ansible-role-configure_sshd](https://github.com/glillico/ansible-role-configure_sshd)<br>
- [ansible-role-copy_etc_issue](https://github.com/glillico/ansible-role-copy_etc_issue)<br>
- [ansible-role-configure_sudo](https://github.com/glillico/ansible-role-configure_sudo)<br>
- [ansible-role-set_hostname](https://github.com/glillico/ansible-role-set_hostname)<br>
- [ansible-role-update_pkgs](https://github.com/glillico/ansible-role-update_pkgs)<br>
- [ansible-role-auto_pkg_updates](https://github.com/glillico/ansible-role-auto_pkg_updates)<br>
- [ansible-role-setup_users](https://github.com/glillico/ansible-role-setup_users)<br>

## Dependencies

This playbook depends on all roles listed in the requirements.yml file.

## License

MIT

## Author Information

This role was created in 2020 by Graham Lillico.
