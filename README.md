# piping-server-http2-docker-compose

[Docker Compose](https://docs.docker.com/compose/) for [Piping Server](https://github.com/nwtgck/piping-server) over HTTP/2 powered by [nghttp](https://github.com/nghttp2/nghttp2)

## Run

```bash
# Create self-signed SSL certificates in ./docker_volumes
./create_ssl_certs.sh
# Run a server
docker-compose up
```

Then, servers run on <http://localhost:8080> and <https://localhost:8443>


## Hierarchy of SSL certificates

You can put your own valid SSL certificates not self-signed ones.

```txt
docker_volumes/
└── ssl_certs
    ├── server.crt
    ├── server.csr
    └── server.key
```
