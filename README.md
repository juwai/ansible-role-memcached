Ansible Role: Memcached
=========

Install memcached libraries on CentOS servers. Install memcached instance is optional.

Requirements
------------

Written in Ansible 1.9.*

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

### force_install_memcached

Install memcached without check `env`.

Default is `no`.

Note: set it to True will also add `juwai.common` as dependency.

### env

Install memcached when env is `vagrant`.

Note: set it to `vagrant` will also add `juwai.common` as dependency.

Dependencies
------------

juwai.common, when `env` is `vagrant` or `force_install_memcached` is `True`.

Example Playbook
----------------

    - hosts: servers
      roles:
         - juwai.memcached

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2016 by [Juwai Limited](http://www.juwai.com).
