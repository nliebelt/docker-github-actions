[![Docker](https://github.com/nliebelt/docker-github-actions/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/nliebelt/docker-github-actions/actions/workflows/docker-publish.yml)

# Docker github actions showcase

Showcase to build and publish a Container with github actions

Main purpose is to give an example for publishing container images vi github ci

## Build

Build a local container from the `Dockerfile`

```shell
docker buildx build . --file Dockerfile --tag artifacts.serie-a.de:4480/nliebelt/docker-github-actions:latest
```

## Publish

```shell
docker login artifacts.serie-a.de:4480
docker push artifacts.serie-a.de:4480/nliebelt/docker-github-actions:latest
```