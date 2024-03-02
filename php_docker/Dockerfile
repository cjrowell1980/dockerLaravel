FROM php:8.2-fpm

# Install dependencies for PHP modules
RUN apt update && \
    apt install -y zip libzip-dev libpng-dev libicu-dev libxml2-dev

# Install additional PHP modules
RUN docker-php-ext-install mysqli pdo pdo_mysql gd zip intl xml

# Clean APY Cache
RUN apt clean