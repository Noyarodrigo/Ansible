Ubuntu
=========

Minimum and standard configuration for an ubuntu instance.

Requirements
------------
Requires the hosts to be reacheble with ssh (ansible) and that has python installed. 

Role Variables
--------------
Doesn't use default variables

hostname: <you need to specify the hostname for the host/s> 
user_name:
user_password:
paquetes: ['htop', 'tcpdump', 'mtr'] <--- add packages as a list (like in python) 


Dependencies
------------
- None

Example Playbook
----------------

  - name: Starting ubuntu conf
    hosts: webservers
    become: yes 
    roles:
      - role: ubuntu_basic_conf

License
-------

BSD

Author Information
------------------

20/09/2022 -Rodri-
