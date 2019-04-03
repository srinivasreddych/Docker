FROM centos
RUN yum install httpd -y
COPY index.html /var/www/html/

ENTRYPOINT ["/usr/sbin/httpd"] 
CMD ["-D", "FOREGROUND"]
EXPOSE 80
