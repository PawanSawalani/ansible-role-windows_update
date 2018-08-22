windows_update
=========

Ansible role to search for windows updates, install the updates and then reboot the server when reboot is required after installing the updates.

Requirements
------------

The target Windows machines must have whitelisted network access to download updates.

Role Variables
--------------

By default, this role installs the default categories of updates provided by the Ansible win_updates module. Change win_updates_category_names to install alternate categories of updates.

Dependencies
------------

None.

Example Playbook
----------------
```
- hosts: all
  tasks:
  - name: Run Windows Updates.
    include_role:
     name: pawansawalani.ansible_role_windows_update
```
License
-------

BSD

