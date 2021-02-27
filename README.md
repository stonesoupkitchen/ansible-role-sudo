[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/H2H43P9OI)

# Ansible role: sudo

An Ansible role for configuring sudo on Linux systems.

## Requirements

TODO.

## Role Variables

* `sudo_package`: The sudo package, by name. Use `sudo=ver` to pin to a version.
  Defaults to `sudo`.
* `sudo_package_state`: The install state of the sudo package. Defaults to
  `present`.

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

