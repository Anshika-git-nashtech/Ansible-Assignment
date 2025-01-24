#Ansible Playbook for Installing Java and MySQL

~Overview
This Ansible playbook installs OpenJDK 8 and MySQL on an Ubuntu system. MySQL installation only occurs if Java is successfully installed

~Files

-inventory.ini: Defines the target hosts.

-main.yml: The main playbook that installs Java and MySQL.

-dependencies.yml: Secondary playbook that installs MySQL (only if Java installation succeeds).

-roles/: Contains the roles for installing Java and MySQL.

~Running the Playbook

ansible-playbook -i inventory.ini main.yml --ask-become-pass

This installs Java and MySQL sequentially.
