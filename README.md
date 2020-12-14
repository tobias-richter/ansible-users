# tobias_richter.users

[![Build Status](https://github.com/tobias-richter/ansible-users/workflows/CI/badge.svg)](https://github.com/tobias-richter/ansible-users/actions)

This role manages users (including, passwords and ssh keys) on linux systems.

## Requirements

This role requires Ansible 2.7 or higher.

## Role Variables

See [defaults/main.yml](defaults/main.yml) for the documented role variables.

## Example Playbook

This playbook creates a user named john_doe with no password and the primary group john_doe.

    - hosts: users
	  roles:
	    - role: tobias_richter.users
          users_default:
            - name: john_doe
