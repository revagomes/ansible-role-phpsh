# Ansible Role: phpsh

[![Build Status](https://travis-ci.org/revagomes/ansible-role-phpsh.svg?branch=master)](https://travis-ci.org/revagomes/ansible-role-phpsh)

Installs [phpsh](http://www.phpsh.org/). A read-eval-print-loop for php.

## Requirements

PHP must already be installed on the server.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    phpsh_path: ''
    phpsh_repo_source: ''
    phpsh_repo_branch: ''

## Dependencies

  - nbz4live.php-fpm

    or

  - geerlingguy.php

## Example Playbook

    - hosts: webservers
      vars_files:
        - vars/main.yml
      roles:
        - { role: revagomes.phpsh }

*Inside `vars/main.yml`*:

    phpsh_path: ~s/phpsh

## License

MIT / BSD

## Author Information

This role was created in 2015 by [Renato Vasconcellos Gomes](http://revagomes.com.br/).
