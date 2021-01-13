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

Example Playbook (tests/test.yml)
----------------

- name: "Test docker installation in a debian system"                                         
  hosts: test
  become: true 
  roles:                                                                        
                                                                                
    - role: abhisheksafui.docker_debian  

Example Inventory (tests/inventory)
-------------------

[test]                                                                          
192.168.1.100                                                                
                                                                                
[all:vars]                                                                      
ansible_connection=ssh                                                          
ansible_ssh_user=admin                                                  
ansible_ssh_pass=password 


Test
------

ansible-playbook -i inventory ./test.yml --extra-vars "ansible_sudo_pass=password"


License
-------

MIT

Author Information
------------------

I am learning Ansible and trying to automate tasks that I perform repeatedly on
a large number of systems, using ansible.
