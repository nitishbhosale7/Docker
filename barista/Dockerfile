FROM ubuntu:latest
LABEL "Author" = "Nitish"
LABEL "Project" = "Barista_site"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update
RUN apt install apache2 git -y
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD barista.tar.gz /var/www/html