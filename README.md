# ansible-role-icinga2_win_agent

[![Build Status](https://travis-ci.org/chrnie/ansible-role-icinga2_win_agent.svg?branch=master)](https://travis-ci.org/chrnie/ansible-role-icinga2_win_agent)

Install icinga2 on Windows and registers at icingaweb2/director. You must provide a self api key.
This key can be set in director.
Todo: import groups with key on extended kickstart

## Example Playbook
You can find an example playbook for testing purposes on https://github.com/chrnie/icinga2-vagrant-ansible

    - hosts: windows
      vars:
        - icinga2_master_fqdn: icinga2.example.org
        - icinga2_powershell_module_url: https://raw.githubusercontent.com/Icinga/icinga2-powershell-module/master/Icinga2Agent/Icinga2Agent.psm1
        - icinga2_self_api_key: 4693cc050e48862c310531b48dab97bddb1f51ac
      roles:
        - chrnie.icinga2_win_agent

## License

GPLv3

## Author Information

Created in 2017 by Christoph Niemann, https://github.com/chrnie

