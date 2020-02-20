simple-bootstrap
=========

Little role to install packages on test plattforms for further development.

Requirements
------------

To execute:
* Ansible >= 2.7

To execute tests:
* Molecule == 2.22
* LXD

Role Variables
--------------

The items under _simple_bootstrap_pre_packages are a short set of important
packages for me.(python3, unzip).
Use the simple_bootstrap_packages variable for additional packages.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - { role: simple_bootstrap }
      vars:
        simple_bootstrap_packages:
          - nano
```


License
-------

GPLv2

Etc
------------------

Feedback is appreciated. I like to improve my understanding in Ansible
related topics.

ToDo
----
- [ ] Enhance list of important packages.
- [ ] Improve molecule scenario for diffrent plattforms.
- [ ] Error handling.
