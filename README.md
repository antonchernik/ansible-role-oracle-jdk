Oracle JDK
=========

Ansible role for installing Oracle JDK. Tested platforms are:
* Debian 8
* Ubuntu 16

Requirements
------------

Debian 8 (jessie)
Ubuntu 16 (xenial)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Parameter | Required | Default | Choices | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| default_download_directory | yes | /tmp | | Sets directory where files will be downloaded |
| jdk_tarball_url  | yes | http://download.oracle.com/otn-pub/java/jdk/8u161-b12/2f38c3b165be4555a1fa6e98c45e0808/jdk-8u161-linux-x64.tar.gz | | Sets Oracle JDK tarball url  |
| jdk_tarball_file | yes  | jdk-8u161-linux-x64 | | Sets Oracle JDK tarball file name |
| jdk_tarball_directory | yes  | jira | jdk1.8.0_161 | Sets Oracle JDK extract directory |
| java_home_directory | yes  | /usr/lib/jvm | | Sets path to JAVA_HOME |

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
