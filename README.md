ansible-role-service
====================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-service.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-service)

Manage services for CentOS 7 and Ubuntu 18.04

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

    - name: Start and Enable sshd
      hosts: service
      become: yes
      become_method: sudo
    
      vars:
        - service:
          - name: sshd
    
      roles:
        - ansible-role-service

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)