FROM php:7.1-fpm

# install modules
RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libmcrypt-dev \
        libpng12-dev \
        libicu-dev \
        wget \
        git \
            --no-install-recommends

RUN docker-php-ext-install mcrypt zip intl mbstring pdo_mysql exif \
    && docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ \
    && docker-php-ext-install gd

COPY php.ini /usr/local/etc/php/

EXPOSE 80