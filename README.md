![Ansible Lint](https://github.com/johanneskastl/ansible-role-update_all_packages/workflows/Ansible%20Lint/badge.svg)

update_all_packages
=========

Update all packages on a system after a `zypper refresh`/`apt-get update`/`yum makecache`. Reboot the machine afterwards.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

Needs the reboot role to trigger a reboot after applying all updates.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: 'johanneskastl.update_all_packages' }

Note on ansible-lint
-------
ansible-lint warns that package tasks should not use `state=latest`, as this renders the playbook not idempotent. This warning is being ignored in this role.

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
