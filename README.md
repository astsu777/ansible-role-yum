Ansible Role: YUM
=========

This role configures the yum packet manager on CentOS/Red Hat systems. At first, it enables the EPEL repository on the system and update all packages. In addition to this, it enables automatic installation of security updates and provide email notifications.


Requirements
------------

No specific requirements for this role.


Role Variables
--------------

Two variables exist for the role: the first one allows you to choose what kind of updates need to be automatically installed and the other one provides the email address for the notifications to be sent to.

```
update_type: security
notification_email: myaddress@myemail.com

```


The variable can be defined in group_vars or in host_vars.


Dependencies
------------

No dependencies from other roles required.


Example Playbook
----------------

Here is a simple example playbook to use this role:

```
hosts: all
user: root
roles:
  - { role: yum, tags: [ 'yum' ] }
```


License
-------

MIT / BSD

Author Information
------------------

My name is Gaétan. You can follow me on [Twitter](https://twitter.com/gaetanict)

Website: [ICT Pour Tous](https://www.ictpourtous.com)
