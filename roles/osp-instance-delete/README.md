osp-instance-delete
============

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

osp-instance-delete is an ansible role used to delete Openstack instances.

Requirements
------------
It's required a connection to openstack.

Example Playbook
----------------
    - hosts: servers
	  become: yes
      roles:
        - osp-instance-delete

License
-------
GPLv3

Author Information
------------------
This role was created in 2020 by [Gary López](https://github.com/gglm92 "Gary López").
