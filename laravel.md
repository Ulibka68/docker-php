Composer не заупститься если не дать прав на директорию
wsl:
cd /root/_prj/docker-php
chmod 777 sites

команда из под wsl
docker-compose up -d --build
docker-compose down

docker exec -it php bash

composer create-project --prefer-dist laravel/laravel:^7.0 hello