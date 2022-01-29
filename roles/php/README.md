Php
=========

Ansible role which installs / configures php-fpm

Role Variables
--------------

Required variables
```
tcp_socket
```

Optional variables
```
php_version # default value: "7.4"
nginx_document_root # default value: "/var/www/html"
```

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: php
           tcp_socket: "{{ tcp_socket }}"
