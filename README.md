Clickhouse-role
=========

Role describes installation Clickhouse

Requirements
------------

  - src: git@github.com:AlexeySetevoi/ansible-clickhouse.git

Role Variables
--------------

Default vars: clickhouse_version: "22.3.3.44"
Vars: clickhouse_packages:
  - clickhouse-client
  - clickhouse-server
  - clickhouse-common-static

Dependencies
------------
Other used rollers:
vector-role
lighthouse-role

Example Playbook
----------------
- name: install clickhouse
  hosts: clickhouse
  roles:
    - clickhouse
