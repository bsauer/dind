FROM docker:1.12-dind

LABEL org.label-schema.vcs-url="https://github.com/bsauer/dind" \
      org.label-schema.vendor=bsauer.com \
      org.label-schema.name=dind \
      com.bsauer.license=MIT

RUN apk --no-cache update && apk --no-cache upgrade && \
    apk --no-cache add py-pip && \
    rm -rf /var/cache/apk/* && \
    pip install docker-compose && \
    docker-compose --version

COPY entrypoint.sh /usr/local/bin/
ENTRYPOINT ["entrypoint.sh"]
CMD []
