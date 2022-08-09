ARG ALPINE_VERSION=3.16.1

FROM alpine:${ALPINE_VERSION}

RUN apk add --no-cache dnsmasq

EXPOSE 53 53/udp

ENTRYPOINT ["/usr/sbin/dnsmasq", "-k"]