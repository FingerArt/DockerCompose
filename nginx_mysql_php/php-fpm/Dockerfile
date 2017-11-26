FROM php:5.6-fpm

RUN apt-get update && apt-get install -y --no-install-recommends \
            libz-dev \
            libpq-dev \
            libjpeg-dev \
            libpng12-dev \
            libfreetype6-dev \
            libssl-dev \
            libmcrypt-dev

RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

RUN docker-php-ext-install iconv mcrypt

RUN docker-php-ext-configure gd --enable-gd-native-ttf --with-jpeg-dir=/usr/lib --with-freetype-dir=/usr/include/freetype2 && \
    docker-php-ext-install gd