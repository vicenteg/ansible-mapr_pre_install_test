mapr_pre_install_test
=========

Pre-installation tests, carried out via ansible.

Requirements
------------

None

Role Variables
--------------

You'll want to make sure mapr_disks is set to the list of disks you want to use for MapR FS. These tests are destructive, so hopefully you're reading this before running it.

Dependencies
------------

Example Playbook
----------------

    - hosts: cluster
      roles:
         - { role: mapr_pre_install_test, mapr_disks: [ "/dev/xvdf", "/dev/xvdg" ] }

License
-------

MIT

Author Information
------------------

Vince Gonzalez
