MongoDB Ansible Role
====================
This role installs a very limited MongoDB server. Please don't use it in any kind of production environmet, it's only meant to be used for development purposes.

Requirements
------------
None

Role Variables
--------------
This role requires the following variables to be defined elsewhere in the playbook that uses it:
```yaml
    mongo_user:           mongodb         # MongoDB username
    mongo_password:       mongodb         # MongoDB password
    mongo_db:             yourdb          # MongoDB database name
```
Dependencies
------------
None

Example Playbook
----------------
Register the role in requirements.yml:
```yaml
    - src: capitanh.mongodb-ansible-role
      name: openldap
```
Include it in your playbooks:
```yaml
    - hosts: servers
      roles:
      - mongodb
```
License
-------
BSD

