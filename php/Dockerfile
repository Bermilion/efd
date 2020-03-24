FROM php:7.1-fpm
RUN apt-get update
RUN apt-get install -y libicu-dev libpng-dev
RUN docker-php-ext-install mbstring json intl gd pdo pdo_mysql mysqli

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN alias composer="php /usr/local/bin/composer"
