FROM socifi/php:7.1-fpm

LABEL maintainer "code@socifi.com" description "SOCIFI Development Team"

RUN pecl install xdebug \
    && apt-get install -y libxslt-dev \
    && docker-php-ext-install xsl

RUN composer global require \
    "squizlabs/php_codesniffer=*" \
    "pdepend/pdepend=*" \
    "phpmd/phpmd=@stable" \
    'behat/behat=*' \
    "phpunit/phpunit=6.*" \
    "phploc/phploc=*" \
    "sebastian/phpcpd=*" \
    "theseer/phpdox=*"

# Make Composer binaries/tools reachable
ENV PATH /root/.composer/vendor/bin:$PATH

COPY config/php.ini /usr/local/etc/php/
COPY config/conf.d /usr/local/etc/php/conf.d
