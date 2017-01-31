# Minimal Node Docker File

[![](https://images.microbadger.com/badges/image/temandodx/minimal-node.svg)](https://microbadger.com/images/temandodx/minimal-node "Click for more information.")
[![](https://images.microbadger.com/badges/version/temandodx/minimal-node.svg)](https://microbadger.com/images/temandodx/minimal-node "Click for more information.")
[![](https://img.shields.io/docker/pulls/temandodx/minimal-node.svg)](https://hub.docker.com/r/temandodx/minimal-node "Click for more information.")
[![](https://travis-ci.org/temando/docker-minimal-node.svg?branch=master)](https://travis-ci.org/temando/docker-minimal-node "Click for more information.")

This project contains the Docker file to install node modules for projects. The official [Node 4 image based on Alpine Linux](https://hub.docker.com/_/node/) installation with [Yarn](https://yarnpkg.com) added for convenience.

## Prerequisites

Install [Docker](https://www.docker.com) to run `docker` commands.

## Building the Docker Image

To build the image, run:

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
