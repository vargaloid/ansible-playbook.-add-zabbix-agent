# ansible-playbook.zabbix-agent
ansible-playbook. Add and configure zabbix-agent.

Zabbix-agent 4.4 for CentOS 7; Debian 8 (jessie); Debian 9 (stretch); Debian 10 (buster), Ubuntu 16.04 (xenial), Ubuntu 18.04 (Bionic Beaver)

Only for fresh installation!

You have to modify:
* zabbix-agent.yml --- "remote_user", "hosts", "zbx_srv"

Run: ansible-playbook zabbix-agent.yml --ask-sudo-pass

Version 0.07
 - version of zabbix-agent changed to 4.4

Version 0.06
 - version of zabbix-agent changed to 4.0
 - added Debian stretch, buster; Ubuntu xenial, bionic beaver

Version 0.05
 - changed installtion zabbix-agent version from 3.2 to 3.4
 - Zabbix Vulners plugin installation
 - yml file was rename to zabbix-agent.yml

Version 0.04
 - added zabbix-agent installation
 - modified zabbix user
 - modified zabbix_agentd.conf
 - create scripts dir
 - main script moved to roles/zabbix.agent/tasks/main.yml

Version 0.03
 - added disrtibution version

Version 0.02
 - added ping hosts
 - added debug message with OS
