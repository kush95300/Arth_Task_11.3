# Task 11.1

## Description:

 11.3 Restarting HTTPD Service is not
idempotence in nature and also consume more
resources suggest a way to rectify this challenge
in Ansible playbook

## Solution

created playbook for this:

- custom_apche_server_with_reload.yml : PLAYBOOK to create apche-server with custom port and root directory with idempotance
- delete_custom_web_server.yml   : PLAYBOOK to delte whole setup 
- paramenter.yml  :   CONTAINS required paramenters
- setting.conf    :   CONFIGURATION file for custom changes 


<b>

Imp: First make group in inventory with tag as webserver. Then play this playbook.

---
Inventory:

[webserver]
ip0 ...  ... ....
ip1 ... ... ...
ip2 ... ... ...
ip3 ... ... ..

...




Command : ansible-playbook custom_apche_server_with_reload.yml 
</b>

#NOTE: System should have pip and ansible before running this playbook. 

Thank You 


CREATER: Kaushal Soni

