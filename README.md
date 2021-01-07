Role Name
=========

Ansible role to install docker in a debian system. This role automates the steps
mentioned at https://docs.docker.com/engine/install/debian/ which one would 
otherwise follow and repeat manually to install docker every time in a new debian
system. 

Requirements
------------

NA

Role Variables
--------------

NA

Dependencies
------------

NA

Example Playbook
----------------

- name: "Test docker installation in a debian system"                                         
  hosts: test 
  roles:                                                                        
                                                                                
    - role: /home/abhi/code/ansible/roles/docker_debian  

License
-------

MIT

Author Information
------------------

I am learning Ansible and trying to automate tasks that I perform repeatedly on
a large number of systems, using ansible.
