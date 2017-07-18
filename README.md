Role Name
=========

Install and configure filebeat for sending bounce logs to logstash

Requirements
------------

Debian Jessie

Role Variables
--------------

* logstash_host
* logstash_port


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: mail-server
      roles:
         - { role: ansible-role-filebeat-postfix-bounce, logstash_host: 'logs', logstash_port: 5044 }

License
-------

MIT
