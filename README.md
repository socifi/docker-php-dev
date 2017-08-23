# PHP-FPM with Xdebug and other DEV tools
## Supported tags and respective `Dockerfile` links
* `7.1-fpm-phpunit6`, `7-fpm-phpunit6`, `latest-phpunit6` [(7.1/fpm-phpunit6/Dockerfile)](https://github.com/socifi/docker-php-dev/blob/master/7.1/fpm-phpunit6/Dockerfile)
* `7.1-fpm`, `7-fpm`, `latest` [(7.1/fpm/Dockerfile)](https://github.com/socifi/docker-php-dev/blob/master/7.1/fpm/Dockerfile)
* `7.1-zts` [(7.1/zts/Dockerfile)](https://github.com/socifi/docker-php-dev/blob/master/7.1/zts/Dockerfile)
* `7.0-fpm` [(7.0/fpm/Dockerfile)](https://github.com/socifi/docker-php-dev/blob/master/7.0/fpm/Dockerfile)
* `5.6-fpm`, `5-fpm` [(5.6/fpm/Dockerfile)](https://github.com/socifi/docker-php-dev/blob/master/5.6/fpm/Dockerfile)

[![dockeri.co](http://dockeri.co/image/socifi/php-dev)](https://registry.hub.docker.com/socifi/php-dev/)

[![](https://images.microbadger.com/badges/image/socifi/php-dev.svg)](https://microbadger.com/images/socifi/php-dev "Get your own image badge on microbadger.com")
[![](https://images.microbadger.com/badges/version/socifi/php-dev.svg)](https://microbadger.com/images/socifi/php-dev "Get your own version badge on microbadger.com")
[![GitHub issues](https://img.shields.io/github/issues/socifi/docker-php-dev.svg "GitHub issues")](https://github.com/socifi/docker-php-dev)
[![GitHub stars](https://img.shields.io/github/stars/socifi/docker-php-dev.svg "GitHub stars")](https://github.com/socifi/docker-php-dev)

Based on the [socifi/php](https://store.docker.com/community/images/socifi/php "socifi/php") image.
This image adds some tools that are necessary for development with PHP.
Also suitable for CI/Build servers like [Jenkins](https://store.docker.com/community/images/socifi/jenkins) and
ready-to-use [Jenkins with Blue Ocean and support for building jobs in Docker](https://store.docker.com/community/images/socifi/jenkins) image.

## Maintained by
[SOCIFI Development Team](https://www.socifi.com)

## Description
The repository is fork of [Shimmi/docker-php-dev](https://github.com/shimmi/docker-php-dev)

## DEV Tools included
* [Xdebug](https://xdebug.org/)
* [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer)
* [PHP Depend](https://pdepend.org/)
* [PHP Mess Detector](https://phpmd.org/)
* [Behat](http://behat.org/)
* [PHPUnit](https://phpunit.de/)
* [PHPLOC](https://github.com/sebastianbergmann/phploc)
* [phpcpd](https://github.com/sebastianbergmann/phpcpd)
* [phpDox](http://phpdox.de/)
