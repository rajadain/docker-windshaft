# docker-windshaft

[![Docker Repository on Quay.io](https://quay.io/repository/azavea/windshaft/status "Docker Repository on Quay.io")](https://quay.io/repository/azavea/windshaft)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/azavea/docker-spark-jobserver/blob/develop/LICENSE)

A `Dockerfile` based off of [`node:0.10-slim`](https://registry.hub.docker.com/_/node/) that installs CartoDB's [Windshaft](https://github.com/CartoDB/Windshaft).

## Usage

First, build the container:

```bash
$ docker build -t azavea/windshaft .
```

From there you can run a container with:

```bash
$ docker run \
    --rm \
    --volume ${PWD}/server.js:/opt/windshaft/server.js \
    azavea/windshaft server.js
```
