# FROM ebispot/ols-indexer:stable AS built
FROM ols-indexer-pbar:latest AS built

RUN apk update && apk add openjdk8

COPY ./logback-spring.xml /tmp/logback-spring.xml
RUN cd /tmp ; jar uf /opt/ols-indexer.jar logback-spring.xml
