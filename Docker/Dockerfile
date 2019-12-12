FROM ubuntu:18.04
RUN apt update && apt install -y nginx
RUN apt install -y unzip
COPY Archive.zip  /var/www/html
WORKDIR /var/www/html
RUN unzip Archive.zip
CMD [/usr/sbin/nginx, -g, daemon off;]
EXPOSE 80
