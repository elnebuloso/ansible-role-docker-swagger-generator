# Ansible Role - Swagger Generator for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-generator.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-generator)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_swagger_generator_state: "started"
docker_swagger_generator_version: "v2.1.6"
docker_swagger_generator_container_name: "swagger-generator"
docker_swagger_generator_web_port: "49161"
docker_swagger_generator_web_name: "swagger-generator.box.entwickl.de"
```

## Example Playbook

```
- hosts: localhost
  vars:
    docker_swagger_generator_web_name: "swagger-generator.box.entwickl.de"
  roles:
    - { role: elnebuloso.docker-swagger-generator }
```

## Dependencies

- `apache2` should be installed and working (you can use the `elnebuloso.apache2` role to install).

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)