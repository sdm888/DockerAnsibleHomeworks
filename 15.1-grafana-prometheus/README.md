# Решение ДЗ №1 по модулю 15

docker-compose.yml для запуска Grafana и Prometheus. При запуске нужно будет указать имя и пароль администратора для Grafana через переменные окружения GF_ADMIN_USER и GF_ADMIN_PASSWORD, например:
```
GF_ADMIN_USER=admin GF_ADMIN_PASSWORD=secret docker compose up -d 
```
