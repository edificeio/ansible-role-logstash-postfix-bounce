Role Name
=========

Install and configure Logstash for receiving postfix bounce logs from filebeat, processing them and sending them to elasticsearch

Requirements
------------

* Debian Jessie
* Java

Role Variables
--------------

* elasticsearch_host
* elasticsearch_port
* filebeat_input_port


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
---
- name: 'Installing and configuring Logstash'
  hosts: logstash-server
  remote_user: root

  roles:
    - role: briancoca.oracle_java7
    
    - role: logstash
      elasticsearch_host: 'elastic.localdomain'
      elasticsearch_port: 9200
      filebeat_input_port: 5044

```

License
-------

3-Clause BSD
