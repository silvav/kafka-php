FROM bitnami/php-fpm:7.4-prod

RUN apt-get update && apt-get install -y \
    autoconf \
    build-essential \
    librdkafka-dev

RUN pecl install rdkafka
