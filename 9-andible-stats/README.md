# Решение ДЗ по модулю 9

Ad-hoc команда Ansible, которая возвращает следующие данные:
- IP-адрес
- Тип ОС
- Версия ОС
- Hostname
- Переменные окружения env

```
ansible all -i hosts.ini -m setup -a 'filter=default_ipv4,distribution,distribution_version,hostname,env'
```