Swapfile
========

[![Build Status](https://travis-ci.org/dochang/ansible-role-swapfile.svg?branch=master)](https://travis-ci.org/dochang/ansible-role-swapfile)
[![Ansible Role](https://img.shields.io/ansible/role/25951.svg)](https://galaxy.ansible.com/dochang/swapfile/)
[![Ansible Role](https://img.shields.io/ansible/role/d/25951.svg)](https://galaxy.ansible.com/dochang/swapfile/)

An ansible role to configure a swap file.

Requirements
------------

None

Role Variables
--------------

  - `swapfile_size` (default: `1G`)
  - `swapfile_location` (default: `/swap`)
  - `swapfile_use_fallocate` (default: `no`)
  - `swapfile_swappiness` (default: `no`)
  - `swapfile_vfs_cache_pressure` (default: `no`)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: dochang.swapfile
          swapfile_size: 1G

License
-------

[MIT](https://dochang.mit-license.org/)

Author Information
------------------

Desmond O. Chang <dochang@gmail.com>
