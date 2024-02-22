# Nginx Role

This Ansible role installs Nginx, configures a custom initial page, and adds a new configuration to listen on port 8080.

## Requirements

- Ansible >= 2.10
- Debian (Buster) or Rocky Linux (8)

## Role Variables

- `initial_page_path`: Path to the custom initial page. Defaults to `templates/default.html`.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - nginx_role
```
