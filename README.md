OAM Ansible
=========
This project focus on a docker-compose deployment solution for SMO/OAM Components.
With respect to OAM the SMO implements the O1-interface consumers. According to the O-RAN OAM Architecture and the O-RAN OAM Interface Specification, the SMO implements a NETCONF Client for configuration and a HTTP/REST/VES server for receiving all kind of events in VES format.

The setup contains an OpenDaylight based NETCONF client, ONAP VES Collector, Strimzi Message bus and O-RAN-SC RANPM.

Requirements
------------
### Resources

The solution was tested on a VM with

- 4x Core
- 16 GBit RAM 
- 50 Gbit Storage

### Operating (HOST) System

```
$ cat /etc/os-release | grep PRETTY_NAME
PRETTY_NAME="Ubuntu 22.04.2 LTS"
```
Please follow the required docker daemon configuration as provided in the following ansible role :

https://github.com/sknrao/ansible-exercises/tree/main/focom/docker/roles/ansible-role-docker

### Docker

```
$ docker --version
Docker version 23.0.1, build a5ee5b1
```
### Docker Compose

```
$ docker compose version
Docker Compose version v2.17.2
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }
