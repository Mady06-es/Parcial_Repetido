FROM debian:12

RUN apt update && apt install apache2

RUN libapache2-mod-php nano

RUN ae2mod rewrite headers expires

WORKDIR /var/www/html

EXPOSE 80

CMD [ "apache2ctl" "-D" "FOREGROUND"]


