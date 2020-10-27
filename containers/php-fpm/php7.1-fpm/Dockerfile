FROM php:7.1-fpm
RUN sed -i "s/httpredir.debian.org/mirrors.aliyun.com/g" /etc/apt/sources.list
RUN sed -i "s/security.debian.org/mirrors.aliyun.com/g" /etc/apt/sources.list
RUN apt-get update && apt-get install -y \
    libmcrypt-dev
RUN docker-php-ext-install pdo pdo_mysql iconv mcrypt
EXPOSE 9000
