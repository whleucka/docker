FROM  php:8.1.0alpha3-fpm-alpine

RUN apk add --no-cache ffmpeg bash zsh

COPY ./php/config/php.ini /usr/local/etc/php/php.ini

#RUN docker-php-ext-install mysqli pgsql sqlite3 pdo pdo_mysql pdo_pgsql pdo_sqlite opcache
RUN docker-php-ext-install mysqli pdo pdo_mysql opcache
