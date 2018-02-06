# osm_apache
######  This repository is for installation of apache web server over CentOS/Redhat/Debian/Ubuntu.
######  By this ansible role we are deploying two virtual hosts with the name of test1.com and test2.com.
######  For accessing domains from local system bind domain name with IP. 

# Example:

######  vim /etc/hosts  
######  IP test1.com  
######  IP test2.com  

## Role Variables

######  Available variables are listed below, along with default values:
 
## The variables provided by this role which are mandatory

######   http_port: 80
######   domain1: test1
######   domain2: test2
######   apachelog: /var/log/apache2
######   httpdlog: /var/log/httpd
######   text1: Hi this is new site test1.com  !!
######   text2: Hi this is new site test2.com  !!
######   deb_conf: /etc/apache2/sites-available
######   red_conf: /etc/httpd/conf.d

## Dependencies

######   None.

## Example Playbook
 
 
```
 - hosts: localhost
   become: yes
   roles:
    - osm_apache 
```

# How to use playbook:

``` ansible-playbook -i inventory apache.yml ```

######  where:

######  -i inventory: is the host infor over which this playbook is going to be install

###### apache.yml: is the file which execute the roles, inside the roles we defined the installation method and the OS distribution types.

###### License

###### MIT / BSD

###### Author Information

###### www.opstree.com

###### blog.opstree.com

