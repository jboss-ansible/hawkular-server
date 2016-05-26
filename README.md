[WIP] Hawkular Services Ansible Role
====================================

To deploy and start Hawkular Services (the server part of Hawkular)

Requirements
------------

Fedora 23 is the only tested platform at this time.

Role Variables
--------------

hawkular_version: 1.0.0.Alpha11
hawkular_name: hawkular-dist-{{hawkular_version}}
hawkular_http_port: 8080
hawkular_bind_address: 0.0.0.0

target_directory: /tmp

Dependencies
------------

No dependency

Example Playbook
----------------

- hosts: localhost
  remote_user: root
  roles:
    - hawkular-services

License
-------

Apache License v2

Author Information
------------------

Thomas Heute - Red Hat
