# Ansible Role: ansible

[![Build Status](https://travis-ci.org/bramford/ansible-role-ansible.svg?branch=master)](https://travis-ci.org/bramford/ansible-role-ansible)

Ansible role that installs ansible from pip or native package management

## Supported Operating Systems

- Debian 7+
- RHEL/CentOS 6+
- Ubuntu 12.04+

## Requirements

- Ansible 2.1+

## Role Variables

See `./defaults/main.yml` for configurable variables and their defaults

## Example playbook

    ---
    - name: Example play
      hosts: all
      roles:
        - { ansible }

## Example playbook (with some optional vars set)

    ---
    - name: Example play with optional vars set
      hosts: all
      roles:
        - { ansible,
            ansible_version: 2.2.0,
            ansible_pip: no
          }

## Add as a submodule to your playbook repo

    git submodule add https://github.com/bramford/ansible-role-ansible.git roles/ansible
