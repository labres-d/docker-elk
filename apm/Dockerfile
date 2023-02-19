ARG ELASTIC_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/apm/apm-server:${ELASTIC_VERSION}

COPY config/apm-server.yml /usr/share/apm-server/apm-server.yml
USER root
RUN chown root:apm-server /usr/share/apm-server/apm-server.yml
USER apm-server