FROM php:8.4
RUN apt-get update&& \
    apt-get install --force-yes \
    unzip

COPY --from=mlocati/php-extension-installer:2 /usr/bin/install-php-extensions /usr/local/bin/

RUN install-php-extensions mysqli
RUN install-php-extensions pdo_mysql
RUN install-php-extensions @composer

COPY --from=composer/composer:2.9.3 /usr/bin/composer /usr/bin/composer

EXPOSE 80
