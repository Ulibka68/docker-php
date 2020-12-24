Не забываем в файле HOSTS добавить:

127.0.0.1 hello.loc

На этом все )

Запускаем терминал, переходим в нашу папку и запускаем команду:

docker-compose up -d

Переходим по адресу http://hello.loc/ и видим, что все работает.

Можно зайти в Docker-контейнер php и запустить bash, и проверить работает ли git и composer, для этого введем команду:

docker exec -it php bash
docker exec -it mysql bash

docker inspect mysql
mysql -u root -p


Завершаем работу командой:

docker-compose down

пересобрать сборку:
docker-compose up -d --build

// phpmyadmin  
http://hello.loc:8081


https://tretyakov.net/post/ustanavlivaem-phpmyadmin-s-pomoshhyu-docker/