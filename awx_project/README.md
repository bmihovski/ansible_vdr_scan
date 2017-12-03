Role Name
=========

Automate the process of VDR and Oscam installation, configuration and channels scanning with AWX

Requirements
------------

Ansible 2.1
tower-cli

Role Variables
--------------

awx_host: - (FQDN or IP address of your AWX
awx_password: - (Password credentials)
awx_username: - (Username credentials)
machine_credentials: - (Machine credentials name for ssh connection)
scm_credentials: - (SCM credentials name for git connection)
template_names: - (Template names to be created)(list)
template_files: - (Playbooks for the templates)(list)             
project_name: - (AWX project name to be created)
inventory_name: - (AWX inventory name to be created)
inventory_group: - (Inventory group to be created)

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: localhost
  gather_facts: false
  roles:
    - awx_project
  vars_files:
    - ./awx_vars.yml

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
