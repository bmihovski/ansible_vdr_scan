Role Name
=========

Automate the process of Oscam compilation

Requirements
------------

Ansible 2.1

Role Variables
--------------

oscam_src: - (Where Oscam source is located)

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- name: Install Oscam
  hosts: receiver1
  gather_facts: false
  roles:
    - oscam_install
  vars:
    oscam_src: /usr/local/src/oscam

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
