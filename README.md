ansible-role-zsh
================

[![Build Status](https://travis-ci.org/luckypool/ansible-role-zsh.svg?branch=master)](https://travis-ci.org/luckypool/ansible-role-zsh)

Install zsh and [prezto](https://github.com/sorin-ionescu/prezto) (optionally).


Requirements
------------

None.

Role Variables
--------------


- `zsh_users` (default `[]`): User list which will change default shell to `zsh`
- `prezto_enabled` (default `no`): Install prezto if you need.


Dependencies
------------

None.

Tested env: 

```
  min_ansible_version: 2.1.0
  platforms:
    - name: Ubuntu
      versions:
        - trusty
```

Example Playbook
----------------

    - hosts: servers
      roles:
        - ansible-role-zsh
      vars:
        zsh_users: [travis]
        prezto_enabled: yes


License
-------

MIT
