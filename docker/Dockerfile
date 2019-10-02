FROM php:7.3-alpine

MAINTAINER mitake <mitake.ck@gmail.com>

ENV PHPMD_VERSION=2.7.0

# # install composer
# RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# install phpmd
RUN curl -L https://github.com/phpmd/phpmd/releases/download/${PHPMD_VERSION}/phpmd.phar > /usr/local/bin/phpmd && \
  chmod +x /usr/local/bin/phpmd

VOLUME ["/src"]
WORKDIR /src

ENTRYPOINT ["phpmd"]
