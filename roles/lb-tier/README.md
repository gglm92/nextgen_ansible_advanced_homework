#lb-tier

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
lb-tier is an ansible role used to install and configure haproxy.

Requirements
------------
It's required a repository enabled on the hosts to install haproxy.

Example Playbook
----------------
    - hosts: servers
	  become: yes
	  gather_facts: false
      roles:
        - lb-tier

License
-------
GPLv3

Author Information
------------------
This role was created in 2020 by [Gary López](https://github.com/gglm92 "Gary López").
