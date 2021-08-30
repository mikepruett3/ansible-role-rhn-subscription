Ansible Role: RHN Subscription
=========

Ansible role to configure subscription settings on Linux Servers. (via either Red Hat Enterprise Subscription Manager, or SpaceWalk Server)

Requirements
------------

The role does not require anyting to run on RHEL and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

``` yaml
username: "myuser"
password: "mypass"
activation_key: "xxxxxxxxxx"
spacewalk_server: "myserver.example.com"
```

```username``` The username for Red Hat Enterprise Subscription Manager account

```password```  The password for Red Hat Enterprise Subscription Manager account

```activation_key```  The activiation key to use with SpaceWalk Server

```spacewalk_server```  The hostname of the SpaceWalk Server

Role variables can be stored with the hosts.yaml file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.rhn-subscription
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3/ansible-role-rhn-subscription)
