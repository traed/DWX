FROM wordpress:latest
RUN apt-get update && apt-get install -y libzip-dev

RUN cd /tmp && \
	curl -sSO https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar && \
	chmod +x wp-cli.phar && \
	mv wp-cli.phar /usr/local/bin/wp

RUN pecl install xdebug
RUN docker-php-ext-configure zip
RUN docker-php-ext-install zip
RUN docker-php-ext-enable xdebug

COPY xdebug.ini /usr/local/etc/php/conf.d/
COPY uploads.ini /usr/local/etc/php/conf.d/
