FROM php:7-fpm

RUN apt-get update
RUN apt-get install -y zlib1g-dev libpng-dev libzip-dev zip libmagickwand-dev --no-install-recommends

RUN pecl install imagick && docker-php-ext-enable imagick
RUN docker-php-ext-install zip
RUN docker-php-ext-install gd
RUN docker-php-ext-install mysqli
RUN docker-php-ext-install exif
