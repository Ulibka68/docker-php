# Сборка для разработки на php
### Состав
* nginx
* php 7.4 (composer, xdebug)
* mysql 8

### Примечание
Не забываем в файле HOSTS добавить:  
127.0.0.1 hello.loc

### Проверка
Переходим по адресу (nginx)
http://hello.loc:8080/  
// phpmyadmin  
http://hello.loc:8081

### Команды Docker
пересобрать сборку:
docker-compose up -d --build

docker exec -it php bash
docker exec -it mysql bash

docker inspect mysql


Завершаем работу командой:
docker-compose down

Перечислить образы Docker на вашем компьютере
docker image ls --all

Перечислите контейнеры на компьютере с помощью:  
docker container ls --all  
или  
docker ps -a

// лог для mysql
docker logs mysql


### Ссылка на прототип
mklink /D J:\_prg\wsl\root \\wsl$\Ubuntu20.04\root\_prj

https://tretyakov.net/post/ustanavlivaem-phpmyadmin-s-pomoshhyu-docker/

