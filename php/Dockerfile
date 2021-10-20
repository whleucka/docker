FROM  php:8.0.5-fpm-alpine

RUN apk add --no-cache ffmpeg bash python2 gettext-dev icu-dev
RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
RUN chmod a+rx /usr/local/bin/youtube-dl

COPY ./php/config/php.ini /usr/local/etc/php/php.ini

RUN docker-php-ext-configure intl
RUN docker-php-ext-install mysqli pdo pdo_mysql opcache intl gettext
