Users
=========

Ansible role which creates new user with ssh key

Role Variables
--------------

Required variables
```
default_user_password
ssh_public_key
```

Optional variables
```
username # default value: user
usergroup # default value: sudo
```

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: users
           tcp_socket: "{{ vault_ssh_public_key }}"
           default_user_password:"{{ vault_user_password }}"
