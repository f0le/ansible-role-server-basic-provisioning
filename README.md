Server-basic-provisioning
=========

This role sets up minimal configuration on a server to use ansible(comfortably).

It creates an ansible user, an ansible group, adds ssh-keys, configures sudo and updates a remote machine.

Requirements
------------

Vps.

Role Variables
--------------

#TODO

add support for ansible vault

----------------

Needed variables:

1. root_password: "$password"
2. ansible_password: "$password"
3. permanent_salt: "$salt" # if a salt is provided for the passwords, hosts won't be "changed" after task completion
4. domain_name: "$domain"


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: basic-server-provisioning }

License
-------

GPLv3

Author Information
------------------

[folie.dev](https://folie.dev)
