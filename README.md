# Ansible role: sudo

An Ansible role for configuring sudo on Linux systems.

## Requirements

TODO.

## Role Variables

TODO.

## Example Playbook

Default usage:

    - hosts: servers
      roles:
         - { role: stonesoupkitchen.sudo }

## Development

Ceate a virtual environment and install modules from requirements.txt:

    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

Enable pre-commit checks:

    pre-commit install

Run molecule tests:

    molecule test

## License

See LICENSE.md

