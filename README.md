ansible-pycon-2013
==================

A set of playbooks to support my talk on Ansible at PyCon India 2013.

setup:

1. Install Ansible 1.3
2. Create a soft link in ansible's library directory to point to the modules directory
3. Make sure hosts specified in the inventory file are accessible via SSH (the playbooks here are very specific to CentOS 6 hosts, but can be modified for other distros/archs as well)

Details about the talk can be found out here:
http://in.pycon.org/funnel/2013/53-ansible-configuration-management-simplified
