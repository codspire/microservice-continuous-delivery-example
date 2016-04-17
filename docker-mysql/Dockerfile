FROM mysql:latest
MAINTAINER Rakesh Nagar <codspire@gmail.com>

RUN echo "0.1" > /version

ENV MYSQL_ROOT_PASSWORD=password

RUN echo "MySQL DB"

#http://stackoverflow.com/questions/22111060/difference-between-expose-and-publish-in-docker
#https://docs.docker.com/v1.5/reference/builder/

#Note: EXPOSE doesn't define which ports can be exposed to the host or make ports accessible from the host by default. 
#To expose ports to the host, at runtime, use the -p flag or the -P flag.

EXPOSE 3306