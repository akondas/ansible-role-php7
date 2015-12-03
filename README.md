# Ansible Role: PHP7

An Ansible role that installs and configure PHP 7 on Debian/Ubuntu servers.

Current PHP7 version: **7.0.0RC8**

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    php_ppa: "ppa:ondrej/php-7.0"    
    php_packages:
      - php7.0-common
      - php7.0-cli
      - php7.0-intl
      - php7.0-curl
      - php7.0-cgi
      - php7.0-fpm
      - php7.0-mysql
      - php7.0-gd
    php_upload_max_filesize: "20M"
    php_post_max_size: "20M"
    php_memory_limit: "1024M"

## Dependencies

None.

## Example Playbook

    - hosts: webservers
      roles:
        - { role: itcraftsmanpl.php7 }

## License

MIT