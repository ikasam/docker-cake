FROM nginx:alpine
MAINTAINER "Masaki Kanno" <ikasam.k503@gmail.com>

RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf
COPY conf.d /etc/nginx/conf.d
