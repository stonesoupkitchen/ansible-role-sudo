[![CI](https://github.com/StoneSoupKitchen/ansible-role-sudo/actions/workflows/ci.yml/badge.svg)](https://github.com/StoneSoupKitchen/ansible-role-sudo/actions/workflows/ci.yml)

# Ansible role: sudo

An Ansible role for configuring sudo on Linux systems.

## Requirements

Supported operating systems:
* Debian 10 (Buster)

## Role Variables

The following table lists all variables that can be overridden
and their default values.

| Name                     | Default Value | Description                      |
| ------------------------ | ------------- | -------------------------------- |
| `sudo_package` | sudo | Name of the sudo package. Use `name=ver` format to pin. |
| `sudo_package_state` | present | Installation state for sudo package. |

## Examples

```yaml
- hosts: all
  roles:
    - stonesoupkitchen.sudo
```

## Development

A Makefile is included for easier development with `pipenv`.
After cloning this repository,
use the following commands to set up an environment.

    pipenv install --dev

To lint your changes with ansible-lint:

    make lint

To run tests with molecule:

    make test

## License

See [LICENSE](./LICENSE).

