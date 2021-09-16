Ansible Role: Python27
========================

Install Python on Amazon Linux 2 or CentOS.

Requirements
------------

Written in Ansible 2.7.*

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

### py_version

Python version, default is `2.7.9`.

### executable_easy_install

`easy_install` executable name, default is `easy_install-2.7`.

### executable_pip

`pip` execuable name, default is `pip2.7`.

### executable_python

`python` executable name, default is `python2.7`.

### python_packages

Additional installed Python packages, default are:

+ `virtualenv`
+ `wheel`

### python_packages_yum

Packages to install when using yum, default are:

+ `python27`
+ `python27-pip`

### python_force_compile

Compile Python from source instead of using yum, default is `false`.

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
