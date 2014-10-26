FROM ubuntu:14.04
MAINTAINER thegreatjerboa

RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get -y install apache2 && \
    echo "<h1>Running from Docker on CoreOS</h1>" > /var/www/html/index.html

EXPOSE 80

ENTRYPOINT ["/usr/sbin/apache2ctl"]
CMD ["-D", "FOREGROUND"]

