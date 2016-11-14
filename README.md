CA certificates
===============

Add additional CA certificates to the trusted certificates list for RHEL/CentOS, Debian/Ubuntu systems.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    ca_certificates: []

List of certificates that will be added to the target system.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      vars_files:
        - vars/main.yml
      roles:
         - gcoop-libre.ca-certificates

*Inside `vars/main.yml`*:

    ca_certificates:
      - custom-ca.crt

License
-------

GPLv2

Author Information
------------------

This role was created in 2016 by [gcoop Cooperativa de Software Libre](http://gcoop.coop).
