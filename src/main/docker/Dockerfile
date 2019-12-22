# Micro Service - Eureka Server
# Author GeekTech
# Version 1.0.0

FROM geekcarnegie/centos:1.0
MAINTAINER GeekTech
VOLUME /tmp
ADD eureka-server-1.0.0.jar eureka-server.jar
RUN bash -c 'touch /eureka-server.jar'
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/eureka-server.jar"]