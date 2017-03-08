# Ansible Role: PHP7

https://galaxy.ansible.com/benlipp/php7/

An Ansible role that installs and configures PHP 7 and Apache on Ubuntu servers.

## Requirements

1. Ansible ([installation instructions](http://docs.ansible.com/intro_installation.html))

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    php_ppa: "ppa:ondrej/php"
    php_packages:
      - php7.0-common
      - php7.0-cli
      - php7.0-intl
      - php7.0-curl
      - php7.0-mysql
      - php7.0-gd
      - php7.0-mbstring
      - php7.0-mcrypt
    php_timezone: UTC
    php_upload_max_filesize: "20M"
    php_post_max_size: "20M"
    php_memory_limit: "512M"
    php_max_execution_time: 60

## Dependencies

None.

## Example Playbook

    - hosts: webservers
      roles:
        - role: benlipp.php7

## License

MIT
