## The Docker LAMP Setup

### Change settings under ```.docker/.env``` ###
##### Available 7.0, 7.1, 7.2 all based on php:alpine docker image

##### Add Host Adress to your /etc/hosts
    echo -e "0.0.0.0 app.doc" | sudo tee -a /etc/hosts

##### Get Git Repository
    git clone https://github.com/aliuosio/mage2.docker.git

##### start docker first time
    cd .docker
    docker-compose  up --build
    
#### after first run (on the everyday bases)
    cd .docker
    docker-compose up -d
    
##### All outgoing mails are sent to MailHog
    https://app.doc:8025

### Todos ###
- set permssions for webserver on php container
- use sockets instead of TCP
- make Database Data persistent
- add Nginx as proxy server
- add xdebug host automatically in php Dockerfile or per bash script