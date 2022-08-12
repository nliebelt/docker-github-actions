[![Docker](https://github.com/nliebelt/docker-github-actions/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/nliebelt/docker-github-actions/actions/workflows/docker-publish.yml)

# Docker publish with GH-Actions and Nexus3

Docker GitHub actions showcase. Build and publish a container with GH-Actions

Main purpose is to give an example for publishing container images via GitHub to an nexus instance.

## Build

Build a local container from the `Dockerfile`

```shell
docker build . --file Dockerfile --tag docker-artifacts.serie-a.de/nliebelt/docker-github-actions:latest
```

## Publish

```shell
docker login docker-artifacts.serie-a.de
docker push docker-artifacts.serie-a.de/nliebelt/docker-github-actions:latest
```
