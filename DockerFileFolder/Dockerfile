FROM docker.io/cenots

RUN yum -y install httpd
COPY index.html /var/www/html

WORKDIR /usr/src/app



EXPOSE 80

CMD apachectl -D FOREGROUND