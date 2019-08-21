FROM huubvdw/docker-nginx-php7:php7.3

RUN set -xe && \
        composer global require hirak/prestissimo && \
        composer clear-cache

COPY entrypoint.sh /usr/local/bin/composer-entrypoint

ENTRYPOINT ["/usr/local/bin/composer-entrypoint"]
