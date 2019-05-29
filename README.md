[![Docker Stars](https://img.shields.io/docker/stars/pr0d1r2/alpine-aria2-command.svg?style=flat-square)](https://hub.docker.com/r/pr0d1r2/alpine-aria2-command/)
[![Docker Pulls](https://img.shields.io/docker/pulls/pr0d1r2/alpine-aria2-command.svg?style=flat-square)](https://hub.docker.com/r/pr0d1r2/alpine-aria2-command/)
[![ImageLayers Size](https://img.shields.io/imagelayers/image-size/pr0d1r2/alpine-aria2-command/latest.svg?style=flat-square)](https://hub.docker.com/r/pr0d1r2/alpine-aria2-command/)

# Alpine Aria2

This image is based on [evild/alpine-base](https://hub.docker.com/r/evild/alpine-base/)

## Version

### Stable

- `stable`, `latest` [(Dockerfile)](https://github.com/pr0d1r2/docker-alpine-aria2-command/blob/master/Dockerfile)
- `1.22.0` [(Dockerfile)](https://github.com/pr0d1r2/docker-alpine-aria2-command/blob/c805baba20115be7e3336931fcb9957aa2c8352e/Dockerfile)

## What is aria2?
aria2 is a utility for downloading files. The supported protocols are HTTP(S), FTP, SFTP, BitTorrent, and Metalink. aria2 can download a file from multiple sources/protocols and tries to utilize your maximum download bandwidth. It supports downloading a file from HTTP(S)/FTP/SFTP and BitTorrent at the same time, while the data downloaded from HTTP(S)/FTP/SFTP is uploaded to the BitTorrent swarm. Using Metalink's chunk checksums, aria2 automatically validates chunks of data while downloading a file like BitTorrent.

## Installation
Automated builds of the image are available on Dockerhub and is the recommended method of installation.
```
docker pull pr0d1r2/alpine-aria2-command:1.22.0
```

You can also pull the latest tag which is built from the repository HEAD : aria2 Mainline with Openssl.
```
docker pull pr0d1r2/alpine-aria2-command:latest
```


## Basic usage
```docker run -p 6925:6925 -p 6888:6888 -e ARIA2_SECRET_TOKEN=mysecretoken --name aria2 pr0d1r2/alpine-aria2-command```
