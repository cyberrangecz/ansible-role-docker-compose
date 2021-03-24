# Ansible role - Docker Compose

This role install Docker Compose.

## Requirements

* This role requires root access, so you either need to specify `become` directive as a global or while invoking the role.

    ```yml
    become: yes
    ```

* Also requires Ansible variables, therefore do not disable directive `gather_facts`.

## Role parameters

No parameters

## Example

The simplest example.

```yml
roles:
    - role: docker-compose
```

