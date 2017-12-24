# Docker
#### Guidelines for writing Dockerfile

FROM baseimage:version
MAINTAINER srinivasreddych@outlook.com
USER root
RUN yum install -y update && \
    yum install x,y,z 
ENV PATH /usr/local/app/bin:$PATH
EXPOSE PortNumber
WORKDIR /app
ADD https://xyz.com /app/
COPY conf /app/conf/
RUN rm -rf needless files
RUN groupadd -g 1000 && useradd -u 1000 && chown -R app:app /app
USER app
CMD python app.py



