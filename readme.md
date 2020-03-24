# Environment for Development
Конфигурация докера для разворачивания web-окружения

Состоит из:
 - nginx
 - php 7.1-fpm
 - composer
 - mariaDB
 - PHPMyAdmin
 
Alias:
 - alias php='docker exec -it php php'
 - alias composer='docker exec -it php composer'
 
Переменные окружения:
 - PATH_TO_SITES — путь до папки с сайтами, которую нужно подключить
 - MYSQL_ROOT_PASSWORD — пароль для root пользователя БД
 - MYSQL_DB_PATH — путь до папки, где будут храниться базы данных (обычно `/var/lib/mysql`)
 - PHP_MY_ADMIN_PORT  — порт для PHPMyAdmin