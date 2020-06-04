osp-facts
============

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

osp-facts is an ansible role used to get information of instances from Openstack and add it to inventory.

Requirements
------------
It's required a connection to openstack.

Example Playbook
----------------
    - hosts: servers
	  become: yes
      roles:
        - osp-facts

License
-------
GPLv3

Author Information
------------------
This role was created in 2020 by [Gary López](https://github.com/gglm92 "Gary López").
