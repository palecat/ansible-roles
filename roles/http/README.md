http
=========

Ansible role which installs / configures nginx

Role Variables
--------------

Required variables
```
tcp_socket
```

Optional variables
```
nginx_port # default value: "80"
nginx_document_root # default value: "/var/www/html"
nginx_index # default value: "index.php"
```

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: http
           tcp_socket: "{{ tcp_socket }}"
