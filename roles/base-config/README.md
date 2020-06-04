#base-config

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

base-config is an ansible role used to enable repositories.

Example Playbook
----------------
    - hosts: servers
	  become: yes
	  gather_facts: false
      roles:
        - base-config

License
-------
GPLv3

Author Information
------------------
This role was created in 2020 by [Gary López](https://github.com/gglm92 "Gary López").
