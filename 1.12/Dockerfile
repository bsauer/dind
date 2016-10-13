FROM docker:1.12-dind

LABEL org.label-schema.vcs-url="https://github.com/bsauer/dind" \
      org.label-schema.vendor=bsauer.com \
      org.label-schema.name=dind \
      com.bsauer.license=MIT

RUN apk update && apk upgrade && apk add py-pip && \
    pip install docker-compose && \
    docker-compose --version

COPY entrypoint.sh /usr/local/bin/
ENTRYPOINT ["entrypoint.sh"]
CMD []
