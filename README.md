# Boilerplates for Automation and Deployment

These are my templates and configurations I use in various projects and deployment scenarios.  
They are based on automation and deployment tools such as Ansible, Docker , Vagrant

# Ansible Role: Docker

Ansible role that installs Docker and Docker Compose.

## Supported Platforms
- Arch Linux
- Debian buster

## Requirements
- Python 3. Python 2 is not supported.

## Role Variables
| Variable                        | Default | Description                                                                              |
|:--------------------------------|:--------|:-----------------------------------------------------------------------------------------|
| **docker_distribution**         |         | **Required**. For which distribution to install Docker. Supports `Archlinux` or `Debian` |
| **docker_compose**              | `true`  | Whether to install Docker Compose.                                                       |
| **docker_ansible_requirements** | `false` | Whether to install requirements for the Ansible Docker modules.                          |
| **docker_users**                |         | A list of users that should be added to the docker group.                                |

## Dependencies
None.

## Example Playbook
```yaml
- hosts: all
  roles:
    - role: acehko.docker
      docker_distribution: Archlinux
      docker_compose: true
      docker_users:
        - user1
        - user2
```

## License
[MIT](LICENSE)

## Author Information
[Mislav Matoković](https://github.com/mmatokovi)