# Docker: Swiss Army Knife

[![GitHub](https://img.shields.io/github/license/wozorio/docker-swiss-army-knife)](https://github.com/wozorio/docker-swiss-army-knife/blob/master/LICENSE)

This repository is used to build a Ubuntu-based docker image containing various tools which are useful for troubleshooting.

## Build the image

```bash
docker build --no-cache -t wozorio/swiss-army-knife:1.0.0 .
```

## Push the image to Docker Hub

```bash
docker login
docker image push wozorio/swiss-army-knife:1.0.0
```

## Run container interactively on Docker

```bash
docker run -it --rm wozorio/swiss-army-knife:1.0.0 /bin/bash
```

## Run pod interactively on Kubernetes

```bash
kubectl run --name -it --rm swiss-army-knife --image=wozorio/swiss-army-knife:1.0.0 -- /bin/bash
```
