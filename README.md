# avto

This crappy thing not for use in production!
Do not build sources with ansible!

Requirements
------------

* Ansible latest
* VirtualBox
* [Vagrant]

Variables
------------

For use with vagrant, can be defined in Vagantfile "ansible.extra_vars". For single use, define somewhere.

* `name`     - Name of package
* `version`  - Package version
* `release`  - Package release
* `arch`     - x86_64

Usage
------------

Define version in spec file == `version`.

    cd build && vagrant up && vagrant halt
    cp *.rpm ../install/files
    cd ../install && vagrant up
    ftp 192.168.33.10

IP address of box defined in Vagrantfile.
