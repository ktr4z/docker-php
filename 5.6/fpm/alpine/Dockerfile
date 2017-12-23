FROM php:5.6-fpm-alpine
RUN apk update \
    && apk add --no-cache libmcrypt-dev \
    && docker-php-ext-install mcrypt pdo_mysql
    # && usermod -u 1000 www-data
WORKDIR /code
