yasarlaro.kvm-cloud-init
=========

Provisions CentOS7 or CentOS8 cloud image with cloud-init

Requirements
------------

You need to have a running libvirt hypervisor.

Role Variables
--------------

Role variables can be found under "defaults" and "vars" directory. There is only one variable that you need to define if you are not changing the defaults: `vm_ip`.
If you do not define `vm_ip` variable, role will fail.

Dependencies
------------

There is no dependency on any other role or module

Example Playbook
----------------

    - hosts: hypervisor
      vars:
        vm_ip: 10.10.10.10
      roles:
         - { role: yasarlaro.kvm-cloud-init }

License
-------

MIT License
