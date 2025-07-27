FROM php:8.4-fpm

# Install system deps
RUN apt-get update && apt-get install -y \
    unzip zip curl git libzip-dev \
    && docker-php-ext-install pdo pdo_mysql zip

# Install Composer
RUN apt-get update && apt-get install -y curl unzip && \
    curl -sS https://getcomposer.org/installer | php && \
    mv composer.phar /usr/local/bin/composer

WORKDIR /var/www/html

RUN mkdir -p /var/www/html/var && \
    chown -R www-data:www-data /var/www/html/var




