FROM alpine:latest
RUN apk upgrade --no-cache && apk add --no-cache ca-certificates mailcap tzdata
RUN adduser -u 1000 -S user

LABEL org.opencontainers.image.source https://github.com/acrobox/docker/tree/master/alpine
