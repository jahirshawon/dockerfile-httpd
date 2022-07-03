FROM centos:7
MAINTAINER Jahir
RUN yum -y install httpd
COPY index.html /var/www/html
RUN echo "ServerName 192.168.0.10" >> /etc/httpd/conf/httpd.conf
EXPOSE 80
#CMD apachectl -D FOREGROUND
CMD ["/usr/sbin/httpd", "-D" , "FOREGROUND"] #runtime with jason format
