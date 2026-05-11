# My Ansible Workspace

A ready-to-use Ansible development environment for OpenShift Dev Spaces.

## What's Included

When you open this repository in Dev Spaces, the workspace automatically provisions:

- **ansible-core 2.17** — pinned to a stable release
- **molecule** — testing framework for Ansible roles
- **ansible-lint** — linting and best practices
- **yamllint** — YAML syntax validation
- Collections: `ansible.posix`, `community.general`

## Quick Start

1. Fork this repository
2. Open it in Dev Spaces (paste the URL in the dashboard)
3. Wait ~2 minutes for tools to install automatically
4. Start writing playbooks in `playbooks/`

## Project Structure

```
├── devfile.yaml          # Dev Spaces workspace definition
├── ansible.cfg           # Ansible configuration
├── inventory/
│   └── hosts.yml         # Inventory (localhost by default)
├── requirements.yml      # Ansible collections to install
├── playbooks/
│   └── hello.yml         # Sample playbook
└── roles/                # Your roles go here
```

## Usage

```bash
# Run the sample playbook
ansible-playbook playbooks/hello.yml

# Lint your code
ansible-lint .

# Create a new role
ansible-galaxy role init roles/my-role
```

## Customization

Edit `devfile.yaml` to change resource limits, add tools, or modify the environment for your team.
