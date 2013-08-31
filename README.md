ansible-pycon-2013
==================

A set of playbooks to support my talk on Ansible at PyCon India 2013.

setup:

1. Install Ansible 1.3
2. Make sure hosts specified in the inventory file are accessible via SSH (the playbooks here are very specific to CentOS 6 hosts, but can be modified for other distros/archs as well)

Using the tags:

To run all tasks which do not require an internet connection
ansible-playbook -i inventory site.yml --tags "offline"

To run all tasks which are dealing with packages (yum as well as pip)
ansible-playbook -i inventory site.yml --tags "packages"

To run all tasks which require an internet connection
ansible-playbook -i inventory site.yml --tags "internet"



Details about the talk can be found out here:
http://in.pycon.org/funnel/2013/53-ansible-configuration-management-simplified
