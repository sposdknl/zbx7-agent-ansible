# Zabbix agent2 a Ansible

Repository pro vyuku na SPOS DK

## Prvni kroky s Ansible

![Zabbix & Ansible](./images/zbx7-ansible.png)

- Red Hat Ansible Automation Platform - [Ansible](https://www.redhat.com/en/technologies/management/ansible)

## Example

```console
vagrant up
vagrant ssh
sudo su -
cd /opt/repo/
ansible-playbook -i inventory.ini -l bastion configure_servers.yml
```

# Požadované známkované úkoly

- Zprovozněte si Zabbix Appliance a nastavte druhou síťovou kartu /etc/sysconfig/network-scripts/ifcfg-eth1
- Upravte URL Vašeho Github Classroom projektu v souboru ansible_provision.yml v Tasku "Cloning Git repository"
- Upravte Ansible playbook pro instalaci Zabbix agenta pro instalaci Agent2 ve verzi 7.0 LTS
- Upravte Ansible playbook pro instalaci Zabbix agenta a Nastavte HostMetadata ( [dokumetace community.zabbix](https://galaxy.ansible.com/ui/repo/published/community/zabbix/docs/ZABBIX_AGENT_ROLE/) )
- 

...

...