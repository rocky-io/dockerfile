FROM hyperf/hyperf:7.4-alpine-v3.15-swoole-v4.8

##
# ---------- building ----------
##
RUN set -ex \
    && apk update \
    && apk add --no-cache \
    php7-pecl-psr \
    php7-phalcon \
    && apk del --purge *-dev \
    #&& apk cache clean \
    && rm -rf /var/cache/apk/* /tmp/* /usr/share/man \
    && php --ri phalcon \
    && echo -e "\033[42;37m Build Completed :).\033[0m\n"