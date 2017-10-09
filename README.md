[![build status](https://gitrep.services.local/ansible-middlewares/ansible-java/badges/develop/build.svg)](https://gitrep.services.local/ansible-middlewares/ansible-java/commits/develop)
Role Name
=========

	This role install Java
	It supports :
		Oracle Java v6 & v7 & v8 (JDK / JRE)
		Open JDK v6 & v7 & v8 (JDK / JRE)
	OS supports : Precise & Trusty

Requirements
------------
	Ansible 2.x

Destination host needs access to aptrepo.services.local.

Role Variables
--------------
## Defaults Vars
	## java_version could be 6, 7 or 8  
	java_version: 8

	## install_jdk could be 0 or 1 ##
	install_jdk: 0

	## install_jre could be 0 or 1 ##
	install_jre: 1
	## Choose between OpenJDK or Oracle Java, if 0 Oracle Java is choosen and if 1 OpenJDK is  ##
	install_openjdk: 0

	## temp_dir is the path where to write temporary file ##
	temp_dir: "/tmp/"

Dependencies
------------

No dependency.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

	- hosts: servers
  		roles:
     		- { role: ansible-java }
  		vars:
    		java_version: 8
    		install_jdk: 0
    		install_jre: 1
    		install_openjdk: 0

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
