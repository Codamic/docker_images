FROM alpine:latest
MAINTAINER devs@codamic.tech

RUN apk apk update
RUN apk apk add nginx
RUN adduser -D -g 'www' www; mkdir /www; chown -R www:www /var/lib/nginx; chown -R www:www /www
COPY ./conf/nginx.conf /etc/nginx/nginx.conf

CMD 'nginx'
