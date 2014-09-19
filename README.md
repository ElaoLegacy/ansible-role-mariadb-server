Ansible Role - MariaDB Server
=============================

A MariaDB Server role to install MariaDB Server on elao symfony standard vagrant box


Requirements
------------

This role only run on elao symfony standard vagrant box. See https://vagrantcloud.com/elao/symfony-standard-debian


Role Handlers
-------------

    mysql server restart  # Restart MariaDB server


Role Variables
--------------

    elao_mysql_users:
      - { name: 'foo', password: 'bar', priv: 'foo.*:ALL', host: '127.0.0.1' }
    elao_mysql_databases:
      - { name: 'foo' }
    elao_mysql_login_user:     root
    elao_mysql_login_password: null
    elao_mysql_login_host:     localhost

    elao_mysql_login_auto: false


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
