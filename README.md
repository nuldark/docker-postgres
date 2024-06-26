# Postgres Docker Container Images

## Supported tags and respective Dockerfile links
- [`16.3`, `16`, `latest`](https://github.com/nuldark/docker-postgres/blob/master/16.3/Dockerfile)
- [`16.2`, `latest`](https://github.com/nuldark/docker-postgres/blob/master/16.2/Dockerfile)
- [`16.1`](https://github.com/nuldark/docker-postgres/blob/master/16.1/Dockerfile)

## Quick reference
- **Image based on**:   
  [alpine:edge](https://hub.docker.com/_/alpine)

- **Supported architectures**:    
  `linux/amd64`, `linux/arm64`

- **Maintained by**:  
  [nuldark](https://github.com/nuldark)

- **Where to file issues**:    
  [https://github.com/nuldark/docker-postgres/issues](https://github.com/nuldark/docker-postgres/issues?q=)

## How to use this image

### start a postgres instance

```console
$ docker run --name some-postgres -d postgres
```

### ... via [`docker-compose`](https://github.com/docker/compose)
Example `docker-compose.yml` for `postgres`:

```yaml
version: '3.1'

services:
    postgres:
        image: nuldark/postgres:latest
        restart: always
        ports:
            - "5432:5432"
```

## Environment Variables

The postgres image uses several environment variables which are easy to miss.

| Variable | Default Value | Description |
|----------|---------------|-------------|
| `PGDATA` |               |             |

## LICENSE

View [license](https://www.postgresql.org/about/licence/) information for the software contained in this image.