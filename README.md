# Ansible Role: restic

[![CI](https://github.com/sgaunet/ansible-role-restic/workflows/CI/badge.svg?event=push)](https://github.com/sgaunet/ansible-role-restic/actions?query=workflow%3ACI)

An Ansible Role that installs [restic][https://github.com/sgaunet/restic] on Linux.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    restic_version: latest"
    restic_os: "linux"
    restic_arch: "amd64"
    restic_release: "https://github.com/restic/restic/releases/download/v{{ restic_version }}/restic_{{ restic_version }}_{{ restic_os }}_{{ restic_arch }}.bz2"

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - sgaunet.restic
```

## License

MIT
