ARG ALPINE_VERSION=3.16.1
ARG DNSMASQ_VERSION=2.86-r3

FROM alpine:${ALPINE_VERSION}

RUN apk update && \
    apk upgrade && \
    apk add dnsmasq=${DNSMASQ_VERSION} && \
    rm -rf /var/cache/apk/*

EXPOSE 53/udp

ENTRYPOINT [ "dnsmasq" ]
