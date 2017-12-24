FROM centos:latest
MAINTAINER srinivasreddych@outlook.com
RUN yum update -y && \
    yum install epel-release -y && \
    yum install nginx -y && \
    echo "daemon off;" >> /etc/nginx/nginx.conf && \
    echo "Starting nginx inside docker on centos base" >> /usr/share/nginx/html/index.html

ENV PATH /usr/local/nginx/bin:$PATH
EXPOSE 80
CMD ["nginx"]
