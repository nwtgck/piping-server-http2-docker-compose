# (base: https://github.com/dit4c/dockerfile-nghttpx)

FROM alpine:3.12
LABEL maintainer="Ryo Ota <nwtgck@nwtgck.org>"

RUN adduser -S -D -h /dev/null -s /sbin/nologin nghttpx && \
    apk --no-cache add nghttp2 tini

ENTRYPOINT ["tini", "--", "nghttpx", "--user=nghttpx"]
