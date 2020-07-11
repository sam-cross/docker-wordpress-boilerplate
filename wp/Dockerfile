# Base on "7.0-apache" tag of php
FROM php:7.4-apache

RUN docker-php-ext-install mysqli
RUN apt-get update \
    && apt-get install -y libzip-dev \
    && apt-get install -y zlib1g-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install zip

# copy src/ directory to /var/www/html
COPY src/ /var/www/html