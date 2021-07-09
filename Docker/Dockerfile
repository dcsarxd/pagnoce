FROM ubuntu:20.04

LABEL dcsar="1.0"

RUN apt-get update && apt-get install nginx --no-install-recommends -y
#RUN apt-get install vim --no-install-recommends -y 
#RUN apt-get install htop --no-install-recommends -y
RUN rm -rf index.nginx-debian.html

WORKDIR /var/www/html

COPY ./templatemo_546_sixteen_clothing ./

CMD [ "nginx", "-g", "daemon off;" ]

