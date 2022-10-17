FROM composer:latest as composer
FROM php:8.0-fpm

# Install modules
RUN apt-get update && apt-get install -y \
	libfreetype6-dev \
	libjpeg62-turbo-dev \
	libpng-dev

RUN docker-php-ext-configure gd --with-freetype --with-jpeg \
	&& docker-php-ext-install gd

RUN docker-php-ext-install mysqli

RUN pecl install --onlyreqdeps --force redis \
	&& rm -rf /tmp/pear \
	&& docker-php-ext-enable redis

CMD ["php-fpm"]
