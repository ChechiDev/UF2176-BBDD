FROM php:7.4-apache
RUN a2enmod rewrite

# Creamos Group & User
# RUN addgroup mi_wordpress && adduser -S -G mi_wordpress wordpress
# USER wordpress  

WORKDIR /var/www/html

COPY wordpress/ .

# Permisos para Apache
RUN chown -R www-data:www-data /var/www/html

# Puerto 80
EXPOSE 80