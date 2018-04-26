FROM wordpress:latest
RUN pecl install xdebug
RUN docker-php-ext-enable xdebug
RUN docker-php-ext-install zip

COPY xdebug.ini /usr/local/etc/php/conf.d/
