FROM armhf/alpine

RUN apk add --no-cache curl

RUN curl -o /usr/bin/minio "https://dl.minio.io/server/minio/release/linux-arm6vl/minio"
RUN chmod 0755 /usr/bin/minio

EXPOSE 9000
ENTRYPOINT ["minio"]
VOLUME ["/export"]
