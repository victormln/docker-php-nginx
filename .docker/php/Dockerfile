FROM php:8.1-fpm

RUN apt-get update && \
    apt-get -y install --no-install-recommends curl gnupg gnupg2 git wget curl libpng-dev libjpeg62-turbo-dev net-tools \
    libssl-dev libcurl4-openssl-dev pkg-config libxml2-dev zlib1g-dev \
    libpq-dev openssh-client rsync libzip-dev libfreetype6-dev libonig-dev

RUN docker-php-ext-install bcmath curl xml mbstring zip pgsql pdo pdo_pgsql intl soap gd

# Install composer
RUN curl -sS https://getcomposer.org/installer -o composer-setup.php \
    && php composer-setup.php --install-dir=/usr/local/bin --filename=composer