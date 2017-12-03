Role Name
=========

Automate the process of VDR and Oscam installation and configuration

Requirements
------------

Ansible 2.1

Role Variables
--------------

vdr_ver: - (VDR version to be installed)
vdr_target_src_dir: - (Where VDR source is located)
vdr_target_plugins_src: - (Where VDR plugins source is located)
vdr_etc_conf: - (Where VDR startup configuration located)
vdr_lib_dir: - (Where VDR post installation libs are located)
oscam_src: - (Where Oscam source is located)

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- name: Install VDR with plugins and deps
  hosts: receiver1
  gather_facts: false
  roles:
    - vdr_install
  vars:
    vdr_ver: vdr-2.2.0
    vdr_target_src_dir: /usr/local/src/VDR
    vdr_target_plugins_src: '{{ vdr_target_src_dir }}/{{ vdr_ver }}/PLUGINS/src'
    vdr_etc_conf: /etc/vdr/conf.d
    vdr_lib_dir: /var/lib/vdr
    oscam_src: /usr/local/oscam

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
