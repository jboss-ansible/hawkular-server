[WIP] Hawkular Services Ansible Role
====================================

To deploy Hawkular Services (the server part of Hawkular)

Requirements
------------

Fedora 23 is the only tested platform at this time.

Role Variables
--------------

hawkular_version: 1.0.0.Alpha11
hawkular_name: hawkular-dist-{{hawkular_version}}
hawkular_http_port: 8080
hawkular_bind_address: 0.0.0.0

download_directory: /tmp
target_directory: /opt

Dependencies
------------

None

Example Playbook
----------------

- hosts: hawkular-services-host
  remote_user: theute
  roles:
    - jboss-ansible.hawkular-services

License
-------

Apache License v2

Author Information
------------------

Thomas Heute - Red Hat
