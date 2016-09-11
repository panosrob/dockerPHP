FROM php:5.6-fpm

ADD php.ini /usr/local/etc/php/conf.d
RUN apt-get update && apt-get install -y libssl-dev \
    && docker-php-ext-install pdo_mysql \
    && pecl install mongodb \
    && echo "extension=mongodb.so" > /usr/local/etc/php/conf.d/docker-php-ext-mongo.ini
