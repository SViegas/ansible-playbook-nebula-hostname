# Ansible Role: Reserve a hostname

An Ansible role that reserves hostname for a VM.

## Requirements

None

## Role variables

The following variables are required by the role.

    vm_generator_ip - The IP address of the hostname generator micro-service
    vm_country - the country name on the hostname (uk, de etc)
    vm_infrastructure - Virtual, Physical, Container (v/p/c)
    vm_os - Linux or Windows (l/w)


## Example Playbook

    - hosts: localhost
      remote_user: root
      roles:
        - ansible-role-reserve-hostname
