awx
=========

    Install Ansible AWX in Docker Compose

Role Variables
--------------

    awx_install:            [default: true] Install common packages, start services
    awx_dir:                [default: /opt/awx] Workdir
    awx_update:             [default: false] Uptade version
    awx_pg_password:        [generated if not present] PostgreSQL password
    awx_admin_password:     [generated if not present] AWX admin password  
    awx_secret_key:         [generated if not present] AWX secret key
    
Example Playbook
----------------

    - hosts: awx
      roles:
        - { name: awx, become: true, tags: awx }

Example Run
-----------

    ansible-playbook awx-compose.yml -i hosts

License
-------

    MIT

Author Information
------------------

    Dmitrij Petrov
