# Ansible role - Docker Compose

This role install Docker Compose.

## Requirements

* This role requires root access, so you either need to specify `become` directive as a global or while invoking the role.

    ```yml
    become: yes
    ```

* Also requires Ansible variables, therefore do not disable directive `gather_facts`.
* Installation of Python package docker-compose requires target Python interpreter version 3.4 or higher.

## Role parameters

Optional.

* `docker_compose_install_python_package` - A boolean value that represents whether to install python package docker-compose
needed by Ansible module docker\_compose or not (default: `True`). This option requires target Python interpreter version 3.4 or higher.

## Example

The simplest example.

```yml
roles:
    - role: docker-compose
```

