Role Name
=========

Automate the process of vdr headless scanning and apply the config

Requirements
------------

Ansible 2.1

Role Variables
--------------

sat_transp_file: /usr/share/dvb/dvb-s/Hellas-39.E
cat_tv_freq_file: /usr/share/dvb/dvb-c/bg-Sprint
vdr_channels_conf_path: /var/lib/vdr/channels.conf
dvb_c_adapter_number: - ( dvb c adapter number )
dvb_s_adapter_number: - ( dvb s adapter number )

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- name: Implement vdr scan sat and catv
  hosts: receiver1
  gather_facts: false
  roles:
    - vdr_scan
  vars:
    - sat_transp_file: /usr/share/dvb/dvb-s/Hellas-39.E
    - cat_tv_freq_file: /usr/share/dvb/dvb-c/bg-Sprint
    - vdr_channels_conf_path: /var/lib/vdr/channels.conf
    - dvb_c_adapter_number: 1
    - dvb_s_adapter_number: 0

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
