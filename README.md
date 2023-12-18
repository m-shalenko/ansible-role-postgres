# ansible-role-postgres

## Purpose
This ansible role installs Postgres in Docker

## Install
```bash
ansible-galaxy role install m-shalenko.postgres
```

## Example of playbook
```yaml
---
- name: Install Postgres
  hosts: postgres
  become: true
  gather_facts: false
  roles:
    - role: m-shalenko.postgres
      tags:
        - postgres
```
