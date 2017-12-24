# Docker
#### Guidelines for writing Dockerfile

1) FROM baseimage:version
2) MAINTAINER srinivasreddych@outlook.com
3) USER root
4) RUN yum install -y update && \
    yum install x,y,z 
5) ENV PATH /usr/local/app/bin:$PATH
6) EXPOSE PortNumber
7) WORKDIR /app
8) ADD https://xyz.com /app/
9) COPY conf /app/conf/
10) RUN rm -rf needless files
11) RUN groupadd -g 1000 && useradd -u 1000 && chown -R app:app /app
12) USER app
13) CMD python app.py



