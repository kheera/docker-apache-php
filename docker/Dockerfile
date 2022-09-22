FROM php:7.2-apache

RUN apt-get update; apt-get install -y \
    vim \
    curl

COPY ./docker/certs/ssl-cert-snakeoil.pem /etc/ssl/certs/
COPY ./docker/certs/ssl-cert-snakeoil.key /etc/ssl/private/

RUN a2enmod ssl
RUN a2ensite default-ssl
