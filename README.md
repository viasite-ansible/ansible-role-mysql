[![Build Status](https://travis-ci.org/viasite-ansible/ansible-role-mysql.svg?branch=master)](https://travis-ci.org/viasite-ansible/ansible-role-mysql)

## Features:
- Install Percona Server
- Configure my.cnf
- Configure pt-kill for kill very long queries
- debops syntax
- ansible lint
- gitlab ci and travis with molecule
- don't remove installed mysql
- percona from ubuntu repo
- all mysql variables wrapped in ansible variables
- fully idempotence
- self-usable with defaults
- setup datadir and debian-sys-maint user

It replaces /etc/mysql/my.cnf and disables conf.d includes, configures only with ansible!

Don't tested with installed mysql.

Playbook deletes ib_logfile when configuration changed, so you can easy change `mysql_innodb_log_file_size`.

## Variables
Role fully customizable, look in [defaults/main.yml](defaults/main.yml).