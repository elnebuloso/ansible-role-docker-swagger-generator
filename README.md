# Ansible Role - Swagger Generator for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-generator.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-generator)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

- [`defaults/main.yml`](https://github.com/elnebuloso/ansible-role-docker-swagger-generator/blob/master/defaults/main.yml)

## Example Playbook

```
- hosts: localhost
  roles:
    - role: elnebuloso.docker-swagger-generator
      docker_swagger_generator_proxy_name: "swagger-generator.box.entwickl.de"
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).
- If Apache2 is installed, a proxy vhost will be configured.

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)