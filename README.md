# RMP ITMO

### ENV 
Docker compose конфигурация для локального поднятия бэкенда (Redis, PgSQL, JVM, Nginx, Prometheus, Graphana)
Её можно склонить в папку docker backend-а там уже добавлен .gitignore и градл настроен чтобы по build таску скидывать jar-ники внутрь этой папки

### CI
Штука которая будет слушать web-хуки гитхаба для автоматического редплоя бека

### Frontend 
Android приложение

### Backend 

### Как работаем

Во всех репах отключены пуши в мастер, для работы:

1. Кусаем от мастера ветку
2. Работаем
3. Открываем PR в мастер, апруваемся, заливаем изменения

Commit convention

```
<type>(<scope>): <short-description>

<description> <--- Опционально
```
**type:**
1. feat - новая функциональность
2. fix - исправление багов
3. build - изменения в коде не затрагивающие функциональность

**scope** - в какой части \ модуле произошло изменение

**short-description** - краткое описание изменений

**description** - развернутое описание, если нужно

Примеры:
```
build(conf): correct configuration examples
```
```
build(core): base project struct, fsm based services, communication between microservices, korm integration
```


