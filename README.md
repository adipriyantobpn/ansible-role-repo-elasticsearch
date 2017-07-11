Ansible Role: ElasticSearch Repository
=========

An Ansible Role that to manage ElasticSearch Yum repository

Requirements
------------

This role needs no special requirements, except sudo access

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):


```yaml
---
repo_location:              international   # available options: international, vagrant
elasticsearch_enabled:      yes
```

Dependencies
------------

None

Example Playbook
----------------

We can use this roles multiple times with different `elasticsearch_version` like this:

```yaml
---
- name: Prepare CentOS 7 server
  hosts: centos7
  roles:
    - role: adipriyantobpn.repo-elasticsearch
      repo_location:              vagrant
      elasticsearch_enabled:      yes
```

License
-------

BSD

Author Information
------------------

This role was created in 2017 by [Adi Priyanto](https://github.com/adipriyantobpn) as a learning purpose for community.