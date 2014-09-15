Ansible Role - MariaDB Server
=============================

A MariaDB Server role to install MariaDB Server on elao symfony standard vagrant box


Requirements
------------

This role only run on elao symfony standard vagrant box. See https://vagrantcloud.com/elao/symfony-standard-debian


Role Handlers
-------------

    mariadb server restart  # Restart MariaDB server


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: elao.mariadb-server }


License
-------

MIT


Author Information
------------------

http://www.elao.com/
