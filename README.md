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

- Zprovozněte si Zabbix Appliance a nastavte druhou síťovou kartu viz /etc/sysconfig/network-scripts/ifcfg-eth1
- Upravte URL Vašeho Github Classroom projektu v souboru ansible_provision.yml v Tasku "Cloning Git repository" pro klonování do VM  Bastion-ansible
- Upravte Ansible playbook pro instalaci Zabbix agenta pro instalaci Agent2 ve verzi 7.0 LTS
- Upravte Ansible playbook pro instalaci Zabbix agenta, nastavte HostMetadata ( [dokumetace community.zabbix](https://galaxy.ansible.com/ui/repo/published/community/zabbix/docs/ZABBIX_AGENT_ROLE/) )
- V Zabbix Appliance vytvoř auto-registrační pravidlo v akcích s HostMetadata
- Nastartuj připravenou VM Bastion-ansible pomoci Vagrant up - upravte dle svého nastavení síť pro propojení se Zabbix Appliance
- Přihlaš se do VM Bastion-ansible a spusť ansible playbook v adresáři /opt/repo pro instalaci a konfiguraci Zabbix agenta viz example
- Vytvoř složku screenshots a config ve svém projektu
- Do adresáře screenshots udělej snímky dokazující pruběh své prace, ansible log, zabbix auto-registracni pravidlo, a registrovaneho hosta + průběh funkčního monitorování atd.
- Do adresáře config vykopiruj konfigurační soubor agenta /etc/zabbix/zabbix_agent2.conf který sestavil Ansible

...
