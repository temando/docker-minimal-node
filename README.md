# Minimal Node Docker File

This project contains the Docker file to install node modules for projects. The official [Node 4 image based on Alpine Linux](https://hub.docker.com/_/node/) installation with [Yarn](https://yarnpkg.com) added for convenience.

## Prerequisites

Install [Docker](https://www.docker.com) to run `docker` commands.

## Building the Docker Image

To build the documentation platform Docker image, run:

```sh
docker build -t {imagename} --build-arg SOURCE_COMMIT=$(git rev-parse --short HEAD) .
```

**Note:**

- `{imagename}` can be any string.
- Syntax shown above works in `bash`.

## Log in to the Docker Image

To log in to the previously built Docker image, run:

```sh
docker run -ti {imagename} sh
```

`{imagename}` can be any string.
