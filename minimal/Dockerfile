FROM ghcr.io/acrobox/docker/alpine:latest

FROM scratch
COPY --from=0 /etc/group /etc/group
COPY --from=0 /etc/passwd /etc/passwd
COPY --from=0 /etc/ssl/certs/ca-certificates.crt /etc/ssl/certs/ca-certificates.crt
COPY --from=0 /etc/mime.types /etc/mime.types
COPY --from=0 /usr/share/zoneinfo/ /usr/share/zoneinfo/
COPY --from=0 --chown=user:nobody /home/user /home/user
COPY --from=0 --chown=user:nobody /home/user /tmp
