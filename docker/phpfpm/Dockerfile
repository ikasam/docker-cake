FROM php:fpm-alpine
MAINTAINER "Masaki Kanno" <ikasam.k503@gmail.com>

RUN apk update && apk --update add tzdata icu-dev
RUN docker-php-ext-install pdo_mysql mysqli mbstring intl
RUN mkdir -p /log/fpm
COPY php.ini /usr/local/etc/php/
COPY php-fpm.d/docker.conf /usr/local/etc/php-fpm.d/docker.conf
COPY php-fpm.d/zzz-www.conf /usr/local/etc/php-fpm.d/zzz-www.conf
