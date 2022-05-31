almaops.docker
==========

This ansible role installs docker

Requirements
------------

This role differs from [https://galaxy.ansible.com/geerlingguy/docker](geerlingguy.docker): it installs docker from your distro's repository, not an omnibus daemon from upstream. This leads to more stability.

It installs **pip** and its docker module automatically.

It's not going to install **docker-compose**.

Also it allows to configure **daemon.json**.

Role Variables
--------------

Look into [./defaults/main.yml](./defaults/main.yml)

Example Playbook
----------------

```
- hosts: servers
  roles:
    - role: almaops.docker

```

License
-------

[MIT License](./LICENSE)


Author Information
------------------
Dmitrii Kashin, <freehck@freehck.com>
