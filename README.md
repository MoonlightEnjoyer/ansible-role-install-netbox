INSTALL-NETBOX
=========

This role installs netbox and its dependencies on a target machine.

!IMPORTANT!
This role modifies nginx configuration (/etc/nginx/nginx.conf file) of the target host!

Requirements
------------
Target host must have tar and unzip packages installed, because the are used by one of the role tasks.

Role Variables
--------------
<!-- A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well. -->

Dependencies
------------

<!-- A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles. -->

Example Playbook
----------------

<!-- Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 } -->

License
-------

BSD

Author Information
------------------

<!-- An optional section for the role authors to include contact information, or a website (HTML is not allowed). -->

Role Installation
=========
Prepare requirements.yml file:

- name: ansible-role-install-netbox
  src: https://github.com/MoonlightEnjoyer/ansible-role-install-netbox.git
  scm: git

------------------
Install role from requirements.yml:
  ansible-galaxy role install -f -r requirements.yml
