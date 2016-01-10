FROM php:7-fpm

MAINTAINER Daniel Pinto <cayan@programmer.net>

# provide additional packages
RUN apt-get update && apt-get install -y wget --no-install-recommends && rm -rf /var/lib/apt/lists/*

# phpunit
RUN wget https://phar.phpunit.de/phpunit.phar && mv phpunit.phar /usr/bin/phpunit && chmod +x /usr/bin/phpunit

# composer
RUN curl -sS https://getcomposer.org/installer | php && mv composer.phar /usr/bin/composer && chmod +x /usr/bin/composer
