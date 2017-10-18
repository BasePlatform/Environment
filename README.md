# Config

Configuration Files of BasePlatform Services

# Commands

Make sure that the port in nginx/conf.d file matches the port you declare in below commands at `-p 80:80` and `SERVICE_PORT=80`

### Start a Docker Dev

docker run -v `/var/www/BasePlatform/App`:/var/www/app -v /var`/www/BasePlatform/Config/nginx/conf.d`:/etc/nginx/conf.d -p `80:80` -e `SERVICE_PORT=80` strong-php7-dev:latest

### Log in to a Docker Dev bin/sh

docker run -it -v `/var/www/BasePlatform/App`:/var/www/app -v `/var/www/BasePlatform/Config/nginx/conf.d`:/etc/nginx/conf.d -p `80:80` -e `SERVICE_PORT=80` strong-php7-dev:latest `/bin/sh`