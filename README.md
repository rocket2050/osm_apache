# This repository is used for apache installation for CentOS/Redhat/Debian/Ubuntu.
In this repo we are deploying two virtual hosts as well by the name of test1.com and test2.com.
For accessing domains from local system bind domain name with IP. 

# Example:
vi /etc/hosts  
IP test1.com  
IP test2.com  

# All the config should be inside role directory which is:
# Role name: 
apache


# How to use playbook:
 ansible-playbook -i inventory apache.yml

where:

-i inventory: is the host infor over which this playbook is going to be install

apache.yml: is the file which execute the roles, inside the roles we defined the installation method and the OS distribution types. 
