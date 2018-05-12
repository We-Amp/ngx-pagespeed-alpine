# ngx-pagespeed-alpine
ngx_pagespeed Dockerfile for Alpine, based on wernight/docker-alpine-nginx-pagespeed

## Docker base
This image is based on Alpine Linux version 3.7

## Pagespeed Components:
### mod-pagespeed
1.13.35.2
### ngx-pagespeed
1.13.35.2
### Nginx
Stable NGINX version 1.14.0 fetched from [nginx.org](http://nginx.org/download) .

This image should be a 100% compatible drop in replacement for the official nginx image.

## Using the Dockerfile
### Use docker build command to build an image from dockerfile:
      $ docker build -t <image_tag> -f <dockerfile_path> .
  Refer [this](https://docs.docker.com/engine/reference/commandline/build/) for additional options.

### Run this container as an independent service:
    $ docker run -d -p 80:80 <image_tag>
  Refer [this](https://docs.docker.com/engine/reference/run/) for additional options.

## Requirements for building:
- > 3 GB of free diskspace
- 2GB of memory
- an x86_64 compatible processor
- Docker CE > 17.3.2

## TODO
- Create a dockerhub repo
