FROM  php:7.4-fpm-alpine

RUN apk add --no-cache ffmpeg bash python2
RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
RUN chmod a+rx /usr/local/bin/youtube-dl

RUN docker-php-ext-install mysqli pdo pdo_mysql
