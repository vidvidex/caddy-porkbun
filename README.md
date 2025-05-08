# Caddy with Porkbun DNS provider

[![Build](https://github.com/vidvidex/caddy-porkbun/actions/workflows/docker-build.yml/badge.svg)](https://github.com/vidvidex/caddy-porkbun/actions/workflows/docker-build.yml)

This is a Docker image for Caddy with the [Porkbun DNS provider](https://github.com/caddy-dns/porkbun/).

The script to rebuild the image is triggered every day to ensure the image is up to date.
To avoid building the image if the base image hasn't changed we store the digest of the base image and only rebuild if it has changed.

Both `linux/amd64` and `linux/arm64` images are built.

## Usage

```bash
docker pull ghcr.io/vidvidex/caddy-porkbun:latest
```

or

```bash
docker pull ghcr.io/vidvidex/caddy-porkbun:CADDY_VERSION
```

where `CADDY_VERSION` is the version of Caddy you want to use. For example, `v2.10.4`.
