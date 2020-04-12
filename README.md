![Ansible Lint](https://github.com/johanneskastl/ansible-role-update_all_packages/workflows/Ansible%20Lint/badge.svg)

update_all_packages
=========

Update all packages on a SUSE/openSUSE system after a `zypper refresh`. Reboot the machine afterwards.

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
         - { role: username.rolename, x: 42 }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
