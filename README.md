Role Name
=========

Ansible role to configure repositories for Midonet and MEM.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

midonet_version: "5.2"
midonet_release: "stable"
openstack_version: "mitaka"
plugin_release: "stable"
mem: False
mem_username: # Provide username if MEM is used
mem_password: # Provide password if MEM is used

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: ansible-midonet-repo
           midonet_version: '5.2'
           midonet_release: 'stable'
           openstack_version: 'mitaka'
           plugin_release: 'stable'
           mem: False
           mem_username: 'midonet'
           mem_password: '*******'

License
-------

Apache 2.0

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
