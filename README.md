# Node creation using LXD and Ansible

The aim of this repo is to provide a simple way to create local compute nodes using LXD and Ansible.
Here is a breakdown of what contains the various files and folders:
- ansible.cfg file: containe the main parameters used by Ansible
- inventory folder: containes the hosts files and variables linked to it
- playbook folder: containes the different playbooks to be run

## How to use this repos?
Clone the repos
```
git clone git@gitlab.com:onmyown-open-source/ansible-lxd-nodes.git
cd ansible-lxd-nodes
```

Localy create LXD nodes:
```
ansible-playbook playbook/lxd-node-creation.yml
```

You will be asked for the number of node you want to create.

Delete created LXD nodes:
```
ansible-playbook playbook/lxd-node-deletion.yml
```