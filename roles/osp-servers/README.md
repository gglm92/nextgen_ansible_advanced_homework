#osp-servers

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

osp-servers is an ansible role used to create Openstack instances to deploy Tier App.

Requirements
------------
It's required a connection to openstack.

Role Variables
--------------
```sh
__osp_servers:
- name: frontend
  cloud: openstack
  state: present
  image: rhel-guest
  key_name: ansible_ssh
  flavor: m1.medium
  security_group: frontend
  meta:
    group: frontends
    deployment_name: QA

- name: app1
  cloud: openstack
  state: present
  image: rhel-guest
  key_name: ansible_ssh
  flavor: m1.medium
  security_group: apps
  meta:
    group: apps
    deployment_name: QA

- name: app2
  cloud: openstack
  state: present
  image: rhel-guest
  key_name: ansible_ssh
  flavor: m1.medium
  security_group: apps
  meta:
    group: apps
    deployment_name: QA

- name: db
  cloud: openstack
  state: present
  image: rhel-guest
  key_name: ansible_ssh
  flavor: m1.medium
  security_group: db
  meta:
    group: appdbs
    deployment_name: QA

```

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
