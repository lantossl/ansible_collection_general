# keep_os_update
=========

A role for keeping Linux operating systems up to date

## Requirements
------------

This role uses ansible builtin modules.

## Role Variables
--------------

| Variable name | default value | Purpose |
|---|---|---|
| reboot_schedule_time | 05:00 | Select the time of scheduled system restarts |

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

## Dependencies
------------

This role doesn't have any role dependencies.

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
- hosts: test_hosts
  #remote_user: root
  gather_facts: true
  become: yes
  roles:
    - keep_os_update
```

## License
-------

GPL

## Author Information
------------------

The role's maintainer:

Slimbarszki Lantos (lantos.sl@itvagyunk.info)

with any issues, please address me at the repository's Github Issues page:
https://github.com/lantossl/ansible_collection_general/issues
