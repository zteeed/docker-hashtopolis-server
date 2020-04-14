FROM php:7.3-apache

RUN apt update && apt install -y git
RUN docker-php-ext-install pdo pdo_mysql mysqli
RUN a2enmod rewrite

COPY config/apache2.conf /etc/apache2/apache2.conf
COPY config/000-default.conf /etc/apache2/sites-available/000-default.conf
COPY config/php.ini /usr/local/etc/php/php.ini

RUN git clone https://github.com/s3inlc/hashtopolis.git && \
    mv hashtopolis /var/www/hashtopolis && \
    chown -R www-data:www-data /var/www/hashtopolis
