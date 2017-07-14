# Ansible role: Raw

Executes raw SSH command using "raw" module. Intention of this role is to provide a way to execute raw commands in roles section of the playbook.
For example to install proper Python version before executing roles.

## Compatibility

This playbook has been tested against Fedora 25.

## Installation 

    ansible-galaxy install hekonsek.raw,0.0

## Example playbook

    - hosts: localhost
      remote_user: root
      roles:
        - { role: hekonsek.raw,0.0, vars: {command: 'yum install -y python'} }

## License

Apache 2.0