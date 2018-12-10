FROM nginx:alpine

RUN apk update && apk upgrade

RUN apk add --update bash

COPY conf/nginx.conf            /etc/nginx/nginx.conf
COPY conf/conf.d/default.conf   /etc/nginx/conf.d/default.conf