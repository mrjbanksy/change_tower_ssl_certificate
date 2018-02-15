Role Name
=========

change_tower_ssl_certificate - Install new Tower SSL certificate and key

Requirements
------------

Ansible Tower should already be installed by the time this role is called. This role can be included at the end of the Tower install playbook.

tower.cert and tower.key should be placed in the files directory of this role. I recommend encrypting them using Ansible Vault

Role Variables
--------------

tower_cert_directory: Where the certificate and key will be placed. Value: /etc/tower/

tower_cert_name: The name of the certificate. Value: tower.cert

tower_key_name: The name of the key. Value: tower.key

Dependencies
------------

No external dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: change_tower_ssl_certificate

License
-------

GPLv3


Author Information
------------------

Jeremy Banks (jbanks@redhat.com)
