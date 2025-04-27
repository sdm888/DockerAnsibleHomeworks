# Решение ДЗ #4

### Сборка образа:
```
docker build -t purpleschool_hw4:latest -f ./Dockerfile .
```

### Запуск контейнера в фоновом режиме:
```
docker run -d --name purpleschool_hw4 purpleschool_hw4:latest
```

### Подключение к контейнеру и проверка результата:
```
docker exec -it purpleschool_hw4 sh
```
```
curl http://localhost:80
```