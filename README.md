# base

[![Current Tag](https://img.shields.io/github/v/tag/dronehippie/base?sort=semver)](https://github.com/dronehippie/base) [![Build Status](https://drone.webhippie.de/api/badges/dronehippie/base/status.svg)](https://drone.webhippie.de/dronehippie/base) [![Join the Matrix chat at https://matrix.to/#/#webhippie:matrix.org](https://img.shields.io/badge/matrix-%23webhippie-7bc9a4.svg)](https://matrix.to/#/#webhippie:matrix.org) [![Docker Size](https://img.shields.io/docker/image-size/dronehippie/base/latest)](https://hub.docker.com/r/dronehippie/base) [![Docker Pulls](https://img.shields.io/docker/pulls/dronehippie/base)](https://hub.docker.com/r/dronehippie/base) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8e7cfc660d1d4786b30993abebcd84f9)](https://www.codacy.com/gh/dronehippie/base/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dronehippie/base&amp;utm_campaign=Badge_Grade)

Drone plugin base image used by all plugins provided by this GitHub organization.

## Docker

Build the images with the following commands:

```console
docker build \
  --label org.opencontainers.image.source=https://github.com/dronehippie/base \
  --label org.opencontainers.image.revision=$(git rev-parse --short HEAD) \
  --label org.opencontainers.image.created=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
  --file docker/Dockerfile.amd64 --tag dronehippie/base .

docker build \
  --label org.opencontainers.image.source=https://github.com/dronehippie/base \
  --label org.opencontainers.image.revision=$(git rev-parse --short HEAD) \
  --label org.opencontainers.image.created=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
  --file docker/Dockerfile.arm --tag dronehippie/base .

docker build \
  --label org.opencontainers.image.source=https://github.com/dronehippie/base \
  --label org.opencontainers.image.revision=$(git rev-parse --short HEAD) \
  --label org.opencontainers.image.created=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
  --file docker/Dockerfile.arm64 --tag dronehippie/base .
```

## Security

If you find a security issue please contact [thomas@webhippie.de](mailto:thomas@webhippie.de) first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

-   [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```console
Copyright (c) 2021 Thomas Boerger <thomas@webhippie.de>
```
