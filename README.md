Oracle JDK
=========

Ansible role for installing Oracle JDK. Tested platforms are:
* Debian 8

Requirements
------------

Debian 8 (jessie)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

jdk_tarball_url: Oracle JDK tarball url

jdk_tarball_file: Oracle JDK tarball file name

jdk_tarball_folder: Oracle JDK extract folder

default_download_path: default download folder


Dependencies
------------

None

Example 
----------------
    ---
    - hosts: all
      roles:
         - { role: antonchernik.oracle-jdk }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2017 by [Anton Chernik](https://github.com/antonchernik).
