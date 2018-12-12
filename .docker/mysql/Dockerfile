FROM mysql:5.7

RUN apt-get update && apt-get upgrade -y && apt-get dist-upgrade -y && apt-get autoremove -y

RUN addgroup --gid 3000 --system app
RUN adduser --uid 3000 --system --disabled-login --disabled-password --gid 3000 app

COPY conf/dev.cnf /etc/mysql/conf.d/dev.cnf

ENV TZ=Europe/Berlin
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone