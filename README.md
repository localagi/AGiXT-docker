# AGiXT-docker [Deprecated]

**Repo deprecated, all work transferred to upstream repo**

Sophisticated docker builds for parent project [Josh-XT/AGiXT](https://github.com/Josh-XT/AGiXT). 

![example workflow](https://github.com/localagi/AGiXT-docker/actions/workflows/publish-docker-test.yaml/badge.svg?branch=main)

Easy setup. Compatible. Tweakable. Scaleable.

Status what's been transferred already
- [ x ] poetry migration
- [ x ] Dockerfile and docker compose updates
- [ x ] Testing with jupyter 

#### Supported platforms
`amd64`, ~~`arm64`~~

#### Supported versions
Containers follow the version scheme of the parent project

`main` (default), `v1.1.57-beta`, etc.

See [Releases](../../releases)

## Prerequisites

* `docker` and `docker compose` are available on your system

## Run

* get `docker-compose.yml` (clone repo, copy or else) 
* Run `docker compose`
* open/refresh `http://localhost:8501` 

### Runtime options
Environment variables to set for the specific service

#### version selection `AGiXT_VERSION`
Prepend, e.g. `AGiXT_VERSION=1.1.57-beta`

### Get the latest builds / update
`docker compose pull`

### Cleanup
`docker compose rm`

## Run a dev environment

Use `docker-compose.dev.yaml` as an additon to 
* directly mount source code into the container (run your modifications)
* automatically restart the container on error


Run `docker compose -f docker-compose.yaml -f docker-compose.dev.yaml up`

## Contributing

When there is a new version and there is need of builds or you require the latest main build, feel free to open an issue

## Problems?

Open an issue on the [Issue Tracker](../../issues)

## Limitations
We cannot support issues regarding the base software. Please refer to the main project page mentioned in the second line of this card.
