# Ansible Collection - acme.mycollection

Workshop collection for Ansible Development Tools.

## Description

This collection provides roles and plugins for automating workspace setup tasks. It was created as part of the Ansible Development Tools workshop.

## Included Content

### Roles

| Role | Description |
|---|---|
| `role_acmecorp_setup` | Creates a structured workspace directory with configurable subdirectories |

## Installation

```bash
ansible-galaxy collection install acme.mycollection
```

Or install from source in development mode:

```bash
ade install -e .
```

## Usage

```yaml
---
- name: Set up development workspace
  hosts: all
  become: false

  roles:
    - role: acme.mycollection.role_acmecorp_setup
```

## License

MIT

## Author Information

ACME Corp
