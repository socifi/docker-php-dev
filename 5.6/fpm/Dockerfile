FROM shimmi/php:5.6-fpm

MAINTAINER Jiří Šimeček <jirka@simecek.org>

RUN apt-get install -y libxslt-dev \
    && docker-php-ext-install xsl

RUN composer global require \
    "squizlabs/php_codesniffer=*" \
    "pdepend/pdepend=*" \
    "phpmd/phpmd=@stable" \
    'behat/behat=*' \
    "phpunit/phpunit=5.*" \
    "phploc/phploc=*" \
    "sebastian/phpcpd=*" \
    "theseer/phpdox=*"

# Make Composer binaries/tools reachable
ENV PATH /root/.composer/vendor/bin:$PATH

RUN pecl install xdebug \
    && echo "zend_extension=$(ls -1 /usr/local/lib/php/extensions/*/xdebug.so)" > /usr/local/etc/php/conf.d/xdebug.ini \
    && echo "xdebug.remote_enable=1" >> /usr/local/etc/php/conf.d/xdebug.ini \
    && echo "xdebug.remote_connect_back=1" >> /usr/local/etc/php/conf.d/xdebug.ini \
    && echo "xdebug.profiler_enable_trigger=1" >> /usr/local/etc/php/conf.d/xdebug.ini
