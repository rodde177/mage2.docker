FROM nginx:alpine

RUN apk update && apk upgrade \
    && apk add --update bash \
    && addgroup -g 3000 -S app \
    && adduser -u 3000 -S -D -G app app

COPY conf/nginx.conf            /etc/nginx/nginx.conf
COPY conf/conf.d/default.conf   /etc/nginx/conf.d/default.conf