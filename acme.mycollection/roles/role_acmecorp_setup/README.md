# role_acmecorp_setup

Creates a structured workspace directory with configurable subdirectories.

## Requirements

- ansible-core >= 2.15

## Role Variables

| Variable | Default | Description |
|---|---|---|
| `role_acmecorp_setup_base` | `/tmp/acme-workspace` | Base directory for the workspace |
| `role_acmecorp_setup_dirs` | `[projects, logs, configs]` | Subdirectories to create |
| `role_acmecorp_setup_config_file` | `settings.yml` | Name of the generated config file |

## Example Playbook

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
