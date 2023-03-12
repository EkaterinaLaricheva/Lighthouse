Lighthouse-role
=========

Role describes installation Lighthouse 

Requirements
------------

Should be installed Nginx
Use templates for config lighthouse
Clone and copy git before install

Role Variables
--------------

Vars:

lighthouse_vcs: https://github.com/VKCOM/lighthouse.git
lighthouse_access_log_name: lighthouse_access
lighthouse_location_dir: ~/home/lighthouse
nginx_user_name: "root"

Dependencies
------------
Other used rollers:

clickhouse-role
vector-role

Example Playbook
----------------

- name: Install lighthouse
  hosts: lighthouse
  roles:
    - lighthouse
