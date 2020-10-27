FROM php:5.6-fpm
RUN sed -i "s/httpredir.debian.org/mirrors.aliyun.com/g" /etc/apt/sources.list
RUN sed -i "s/security.debian.org/mirrors.aliyun.com/g" /etc/apt/sources.list

RUN apt-get update && apt-get install -y \
    build-essential libssl-dev zlib1g-dev libpng-dev libjpeg-dev libfreetype6-dev libmcrypt-dev

RUN docker-php-ext-install pdo pdo_mysql mbstring iconv mcrypt gd
EXPOSE 9000
