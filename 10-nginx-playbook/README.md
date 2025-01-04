# Решение ДЗ по модулю 10

Для запуска Nginx в контейнере Docker нужно скопировать файл hosts.ini.example в файл hosts.ini, затем внести в него собственные настройки и запустить выполнение плейбука Ansible командой:
```
ansible-playbook -i hosts.ini nginx-docker.yml -K
```
