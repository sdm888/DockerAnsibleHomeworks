# Решение ДЗ #5

### Сборка образа:
```
docker build -t purpleschool_hw5:latest -f ./Dockerfile .
```

### Запуск контейнера в фоновом режиме:
```
docker run -d -p 8081:80 --name purpleschool_hw5 purpleschool_hw5:latest
```

### Проверка результата:
```
curl http://localhost:8081