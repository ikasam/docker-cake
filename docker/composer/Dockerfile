FROM composer/composer:alpine
MAINTAINER "Masaki Kanno" <ikasam.k503@gmail.com>

RUN apk update && apk --update add icu-dev
RUN docker-php-ext-install pdo_mysql mysqli mbstring intl
