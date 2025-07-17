# Dockerfile

FROM php:7.4-apache

RUN a2enmod rewrite
RUN docker-php-ext-install mysqli

WORKDIR /var/www/html
COPY wordpress/ .

# Permisos para Apache
RUN chown -R www-data:www-data /var/www/html

# Puerto 80
EXPOSE 80
