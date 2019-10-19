# ACTible

Aura Client Tools (ACT) is a simple library to manage Aura service nodes. 
While today this is limited to LCDN, in the future this may include support
for LMS and possibly others.

ACTible is an ansible module that uses ACT to manage the logical lifecycle
management of Aura service nodes. A service node is instantiated on either
a physical or virtual "machine" already bootstrapped with a Linux distribution
that uses either grub2 or grub-legacy. Tested distributions include CentOS 6,
CentOS 7, and Ubuntu.

The intent of using ansible is to dovetail with the myriad IaaS-like
modules available, which include, but are not limited to, the following:
* Digital Ocean
* OpenStack
* Packet
* ...

The above have been tested. More will be added upon finish tests.

## Base setup on RHEL/CentOS 7
yum install epel-release
yum install ansible
yum instsall python-pip

## Ansible Module Installation

### Module Installation info
[docs](https://docs.ansible.com/ansible/latest/reference_appendices/galaxy.html?extIdCarryOver=true&sc_cid=701f2000001OH7YAAW#the-command-line-tool)

### Digital Ocean droplet Module
[docs](https://docs.ansible.com/ansible/latest/modules/digital_ocean_droplet_module.html#digital-ocean-droplet-module)

### Packet bare metal cloud module
[docs](https://docs.ansible.com/ansible/latest/modules/packet_device_module.html#packet-device-module)

### OpenStack module
[docs](https://docs.ansible.com/ansible/latest/modules/os_server_module.html#os-server-module)

### ACTible module
pip install auraclienttools # ACT
... recipe for installing actible module

## Examples
