yasarlaro.kvm-cloud-init
=========

Provisions CentOS7 or CentOS8 cloud image with cloud-init

Requirements
------------

You need to have a running libvirt hypervisor.

Role Variables
--------------

Role variables can be found under "defaults" and "vars" directory. There is only one variable that you need to define if you are not changing the defaults: vm_ip. 

Dependencies
------------

There is no dependency on any other role or module

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: yasarlaro.kvm }

License
-------

MIT License
