# Решение ДЗ по модулю 12

Для запуска сервисов в Docker Swarm нужно предварительно выполнить следующие действия:

1. Создать секрет с паролем для Postgres:
```
printf "<пароль>" | docker secret create postgres.password -
```
2. Добавить метку для ноды, на которой должен запускаться Postgres:
```
docker node update <имя_ноды> --label-add database=true
```

После этого можно перейти в каталог с файлом docker-stack.yml и запустить сервисы командой:
```
docker stack deploy -c docker-stack.yml hw_app
```