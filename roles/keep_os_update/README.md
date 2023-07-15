# keep_os_update

A role for keeping Linux operating systems up to date.

What does this role makes for you? 

- It keeps your package manager's cache up to date.
- It is upgrades your installed packages at the most recent version.
- It is follows the system requirements for a reboot and schedule a restart at the time you want.
- It is warns the user for the forthcoming restart.

## Requirements

This role uses ansible builtin modules.

## Role Variables

| Variable name | default value | Purpose |
|---|---|---|
| reboot_schedule_time | 05:00 | Select the time of scheduled system restarts |

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

## Dependencies

This role doesn't have any dependencies.

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

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
### Inventory file for a test

```
[test_hosts]
ubuntu ansible_host=192.168.10.204
centos8 ansible_host=192.168.10.201 ansible_user=root
```

## License

GPL

## Compatibility

This rule is tested for the following operating systems:
- Ubuntu 22.04
- Centos 8

This rule is compatible with the following package managers:
- APT
- YUM
- DNF

## Author Information

### The role's maintainer:

Slimbarszki Lantos (lantos.sl@itvagyunk.info)

You can report any issues at the repository's [Github Issues](https://github.com/lantossl/ansible_collection_general/issues) page.