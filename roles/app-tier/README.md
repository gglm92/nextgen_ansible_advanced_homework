#App-tier

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
App-tier is an ansible role used to install Tier App

Requirements
------------
It's required a repository enabled on the hosts to install apache and tomcat.

Role Variables
--------------
| Variable | Description |
| ------ | ------ |
| __tomcat_web_root_directory | Root web directory to install index.html  |
| __tomcat_directory | Tomcat directory to install index.html  |

Example Playbook
----------------
    - hosts: servers
	  become: yes
	  gather_facts: false
      roles:
        - app-tier

License
-------
GPLv3

Author Information
------------------
This role was created in 2020 by [Gary López](https://github.com/gglm92 "Gary López").
