FROM httpd:latest

RUN apt-get update \
    && apt-get upgrade -y \
    && apt-get dist-upgrade -y \
    && apt-get autoclean

COPY conf/httpd.conf /usr/local/apache2/conf/httpd.conf
COPY conf/httpd-vhosts.conf /usr/local/apache2/conf/extra/httpd-vhosts.conf