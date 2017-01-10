FROM shimmi/php:7.0-fpm

MAINTAINER Jiří Šimeček <jirka@simecek.org>

RUN apt-get install -y libxslt-dev \
    && docker-php-ext-install xsl

RUN composer global require \
    "squizlabs/php_codesniffer=*" \
	"pdepend/pdepend=*" \
	"phpmd/phpmd=@stable" \
	'behat/behat=*' \
	"phpunit/phpunit=*" \
	"phploc/phploc=*" \
	"sebastian/phpcpd=*" \
	"theseer/phpdox=*"

# Make Composer binaries/tools reachable
ENV PATH /root/.composer/vendor/bin:$PATH

RUN pecl install xdebug