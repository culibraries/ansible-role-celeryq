Ansible Role Celeryq
=========

This role creates a python celery queue template that can be used to easily integrate with cybercommons framework.

Requirements
------------
1. Ansible

#### Optional:

1. ansible-toolbox


Role Variables
--------------
```
    queue_name (default: cybercomq): Name of workflow package that will be installed
    install_directory (default: PWD): install directory, default is the current directory
```
Dependencies
------------

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - ansible-role-celeryq
```

If you want to run with ansible-toolbox (pip install ansible-toolbox):

1. Clone role

```
    git clone <this repo>
```

2. Run - Be sure to set --extra-vars to your variables.

```  
  ansible-role --extra-vars "queue_name=cybercomq" ansible-role-celeryq

```
or place variables in file(example.json)

```  
  ansible-role --extra-vars '@example.json' ansible-role-celeryd
```

License
-------

TBD

Author Information
------------------

Mark Stacy
