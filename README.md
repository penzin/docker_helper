# docker_helper

A very simple minimal bundle for starting with docker & docker-compose. 
It's cosist of three containers, linked with docker-compose.yml.

## Contents
1. Nginx lastes
2. Php-fpm 7.1
3. MySQL 8

## Install and usage
1. install [Docker](https://docs.docker.com/install/) & [Docker-compose](https://docs.docker.com/compose/install/) to your server
2. Clone this repo to your server
3. Change 'server_name' in nginx/site.conf to your actual ip
4. sudo docker-compose up
5. Open http://[your-actual-ip]:8080.

6. (optional) Change content of app/www/ on host machine if you need.
