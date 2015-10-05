Role Name
=========

This is a role in order to install the targeted mysql version

Requirements
------------

- Ansible 2.0
- Debian 7.0+

Role Variables
--------------

### defaults/main.yml
mysql_use_distrib_version: "{{mysql_use_distrib_version_default}}"

#
mysql_server_version: "{{mysql_server_version_default}}"
mysql_host: "{{ mysql_host_default }}"
mysql_ip: "{{ mysql_ip_default }}" 
mysql_port: "{{mysql_port_default}}"
mysql_jdbc_drivers_version: "{{mysql_jdbc_drivers_version_default}}"
mysql_jdbc_drivers_download_URL : "{{mysql_jdbc_drivers_download_URL_default}}"
mysql_jdbc_drivers_class: "{{mysql_jdbc_drivers_class_default}}"
mysql_xwiki_user: "{{mysql_xwiki_user_default}}"
mysql_xwiki_password: "{{mysql_xwiki_password_default}}"

### vars/main.yml
NTP
 this are defined for various OS, currently only debian-7 has been set

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers 
      vars:
          			
      roles:      
      - {role: ansible-xwiki-mysql}
      

License
-------

BSD, GPLV3

Author Information
------------------
C. Sabourdin inspire by Git-hub & XWiki.org
