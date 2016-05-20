Ansible Role: Python 2.7
========================

Install Python 2.7 on Amazon EC2 or CentOS server.

Requirements
------------

Written in Ansible 2.0.*

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

### version

Python version, default is `2.7.9`.

### easy_install

`easy_install` executable name, default is `easy_install-2.7`.

### pip

`pip` execuable name, default is `pip2.7`.

### python

`python` executable name, default is `python2.7`.

### python_packages

Additional installed python packages, default are:

+ `virtualenv`
+ `wheel`

Dependencies
------------

+ `juwai.common`

Example Playbook
----------------

    - hosts: servers
      roles:
        - juwai.python27

License
-------

MIT

Author Information
------------------

This role was created in 2016 by [Juwai Limited](http://www.juwai.com).
