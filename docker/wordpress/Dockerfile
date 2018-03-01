FROM wordpress:latest
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug

COPY xdebug.ini /usr/local/etc/php/conf.d/