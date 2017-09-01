mc.configure
=========

Configures the installed packages such as dnsmasq & LTSP 

Requirements
------------

The role "mc.installpackages" must be run sucessfully before running this role. 

Role Variables
--------------

{{dhcp_pool_start}} - Starting address of the DHCP pool to be allocated
{{dhcp_pool_finish}} - Last address of the DHCP pool to be allocated

Dependencies
------------

The role "mc.installpackages"

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles: 
         - role: mc.configure
           dhcp_pool_start: 192.168.0.100
           dhcp_pool_finish: 192.168.0.200

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
