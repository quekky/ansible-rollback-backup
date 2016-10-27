list-backups
============

Rollback to previous backup.

Requirements
------------

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about them are as follows.

	dest:
	backup_dir:
	#which version (dir name) to rollback to
	rollback_version:
	#if require to backup the current files
	require_backup: false

Dependencies
------------

None

Example Playbook
----------------

List previous backups:

    - hosts: servers
      roles:
        - role: quekky.rollback-backup
		  dest: /deploy
		  backup_dir: /backup
		  rollback_version: 2016-01-01-000000


License
-------

MIT

Author Information
------------------

quekky
