FROM bitrixdock/php71-fpm:latest

MAINTAINER vitams

ADD ./php.ini /etc/php/7.1/fpm/conf.d/90-php.ini
ADD ./php.ini /etc/php/7.1/cli/conf.d/90-php.ini

RUN usermod -u 1000 www-data

RUN mkdir /tmp/sessions-bitrix/ && chmod 777 /tmp/sessions-bitrix/

WORKDIR "/var/www/bitrix"

EXPOSE 9000
