FROM ubuntu:23.04

RUN apt update && apt install -y nginx

# COPY site /etc/nginx/sites-avaliable/
# RUN ls -n /etc/nginx/sites-avaliable/site /etc/nginx/site-enabled/

COPY burgers-landing /var/www/html

WORKDIR /var/www

EXPOSE 80

# VOLUME /var/www

ENV MYTEST=123

CMD ["nginx", "-g", "daemon off;"]