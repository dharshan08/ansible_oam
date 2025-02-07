OAM Ansible
=========
This project focus on a docker-compose deployment solution for SMO/OAM Components.
With respect to OAM the SMO implements the O1-interface consumers. According to the O-RAN OAM Architecture and the O-RAN OAM Interface Specification, the SMO implements a NETCONF Client for configuration and a HTTP/REST/VES server for receiving all kind of events in VES format.

The setup contains an OpenDaylight based NETCONF client, ONAP VES Collector, Strimzi Message bus and O-RAN-SC RANPM.
Requirements
------------
Resources

The solution was tested on a VM with

    4x Core
    16 GBit RAM
    50 Gbit Storage

Operating (HOST) System

$ cat /etc/os-release | grep PRETTY_NAME
PRETTY_NAME="Ubuntu 22.04.2 LTS"

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
