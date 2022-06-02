FROM  php:8.1.0alpha3-fpm-alpine

#RUN docker-php-ext-install mysqli pgsql sqlite3 pdo pdo_mysql pdo_pgsql pdo_sqlite opcache
RUN docker-php-ext-install mysqli pdo pdo_mysql opcache

COPY cron/crontab /etc/crontabs/root

CMD ["crond", "-f"]
