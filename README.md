# Caddy with Porkbun DNS provider

This is a Docker image for Caddy with the [Porkbun DNS provider](https://github.com/caddy-dns/porkbun/).

The script to rebuild the image is triggered every day to ensure the image is up to date.
To avoid building the image if the base image hasn't changed we store the digest of the base image and only rebuild if it has changed.

Both `linux/amd64` and `linux/arm64` images are built.

## Usage

```bash
docker pull ghcr.io/vidvidex/caddy-porkbun:latest
```
