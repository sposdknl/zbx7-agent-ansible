# Zabbix agent2 and Ansible

Repositories for teaching purposes at SPOS DK

Repository pro vyuku na SPOS DK

## First zbx step with Ansible

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
...