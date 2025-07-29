# ci

A collection of useful re-usable Github Actions workflows

## Docker PR

This is the boilerplate for building a docker image, generally used during PR
runs as a confidence check.

## Docker Build

This is roughly based on the excellent [multi-arch-docker-github-workflow]. It
provides a common pattern for building a docker image and pushing both
linux/amd64 and linux/arm64 images using native runners.

In the past seabird repos used buildx, but this could result in a nearly 10x
slowdown for Rust repos, causing a 4 minute build to become a 40 minute build.

[multi-arch-docker-github-workflow]: https://github.com/sredevopsorg/multi-arch-docker-github-workflow/tree/main
