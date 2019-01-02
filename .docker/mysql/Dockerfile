FROM mysql:5.7

COPY conf/dev.cnf /etc/mysql/conf.d/dev.cnf

ENV TZ=Europe/Berlin

RUN apt-get update && apt-get upgrade -y && apt-get dist-upgrade -y && apt-get autoremove -y \
    && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone