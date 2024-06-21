# ARMv7 Build for Browserless

> [!WARNING]
> Work in progress, not ready to use.

This repository contains a GitHub Action workflow designed to build and push
a Docker image of the [browserless](https://github.com/browserless/browserless)
project for the ARMv7 architecture.

The image is available on Docker Hub:

- [iammedvedev/browserless-arm-base:latest](https://hub.docker.com/r/iammedvedev/browserless-arm-base)
- [iammedvedev/browserless-arm-firefox:latest](https://hub.docker.com/r/iammedvedev/browserless-arm-firefox)

## Usage

### Docker

You can pull and run the ARMv7 browserless image using Docker with the following command:

```sh
docker run -p 3000:3000 iammedvedev/browserless-arm-firefox:latest
```

### Docker Compose

You can also use Docker Compose to run the ARMv7 browserless container.
Create a `docker-compose.yml` file with the following content:

```yml
version: "3"
services:
  browserless:
    image: iammedvedev/browserless-arm-firefox:latest
    ports:
      - "3000:3000"
```
