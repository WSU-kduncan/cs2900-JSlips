Joseph Carusone - Project 4

Two Container Choices: Docker and Podman

## 1. Networking

## A. Docker Networking Modes:
- host: useful to optimize performance
- none: disables all networking. Used for custom networking.
- bridge: (default network driver.) Used when your applications run in stand-alone containers needed to communicate.

Run: ``docker run --add-host=host:ip``

## B. Podman Networking Modes:
- bridge: (default mode) creates a network stack on the network
- none: no networking is set up
- host: uses the hosts network
- container: goes off of another containers network

Run: ``podman run --add-host=host:ip``

## 2. Vulnerability scanners

## A. Dockerfile Linter https://marketplace.visualstudio.com/items?itemName=henriiik.docker-linter
Allows you to use perl, python, or ruby in docker containers.

## B. Aqua Trivy
- Only a few containers can be scanned, those being Docker and Podman.
- The vulnerabilites that can be scanned include Container Images, Rootfs, Filesystem, and Git repos.

