isset.package [![build status](https://gitlab.isset.nl/ansible/isset.package/badges/master/build.svg)](https://gitlab.isset.nl/ansible/isset.package/commits/master)
=========

Ubuntu APT package

Requirements
------------

Ansible 2.5 or above is highly recommended.

Role Variables
--------------

	package_state: installed
	package_name: yourpackage
	package_cache_valid_time: 3600 (overridden by apt_cache_valid_time)
	package_delay: 5
	package_max_retries: 3

Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - { role: isset.package, package_name: htop }

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben@isset.nl>
