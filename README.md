# The Docker LAMP Setup

## Get Git Repository
    git clone https://github.com/aliuosio/mage2.docker.git

## Change settings under ```.docker/.env``` ###

### Available 7.0, 7.1, 7.2 all based on php:alpine docker image

## Add Host Adress to your /etc/hosts
    echo -e "0.0.0.0 app.doc" | sudo tee -a /etc/hosts


## start docker first time
    cd .docker
    docker-compose build
    docker-compose up -d
    
## All outgoing mails are sent to MailHog
    https://app.doc:8025

## Todos ###
* set permssions for webserver on php container
* use sockets instead of TCP
* add xdebug host automatically in php Dockerfile or per bash script
