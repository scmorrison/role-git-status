Role: cns.git-status
========

This role displays git status stdout for git repository located at {{ web_root }}

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name     | Default |                                      |
|----------|---------|--------------------------------------|
| web_root |   ---   | Location of the git repository on the target server |
| system_user |   ---   | Name of the system user context to run `git status` |


Dependencies
------------

Assumes the `git` command is available on target server.

License
-------

GPLv2

Author Information
------------------

Created by [Sam Morrison](https://www.twitter.com/samcns)

Examples
--------

```yaml
---
- name: cns.git-status example
  hosts: all
  roles:
    - cns.git-status
```
