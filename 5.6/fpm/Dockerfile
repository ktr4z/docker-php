FROM php:5.6-fpm

RUN apt-get update && apt-get install -y libmcrypt-dev \
    && docker-php-ext-install mcrypt pdo_mysql \
    && groupadd -r -g 1000 tester \
    && useradd -r -u 1000 -g tester tester

USER tester

WORKDIR /code
