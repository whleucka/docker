FROM php:7.4-fpm-alpine

RUN docker-php-ext-install mysqli pdo pdo_mysql

COPY cron/crontab /etc/crontabs/root

CMD ["crond", "-f"]
