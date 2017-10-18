# ngx-pagespeed-alpine
ngx_pagespeed Dockerfile for Alpine, based on wernight/docker-alpine-nginx-pagespeed

## Docker base
This image is based on Alpine Linux version 3.4

## Pagespeed Components:
### mod-pagespeed
Custom built beta release tarball of mod-pagespeed (mod-pagespeed-beta-1.12.34.3.tar.bz2 uploaded in this repo). This custom tarball includes the upgraded GRPC version(1.4.5) which is required for the Alpine build.
### ngx-pagespeed
Stable ngx-pagespeed version 1.12.34.3 fetched from [ngx pagespeed archive](https://github.com/pagespeed/ngx_pagespeed/archive/v1.12.34.3-stable.tar.gz).
### Nginx
Stable NGINX version 1.12.1 fetched from [nginx.org](http://nginx.org/download/nginx-1.12.1.tar.gz) .

## Using the Dockerfile
### Use docker build command to build an image from dockerfile:
      $ docker build -t <image_tag> -f <dockerfile_path> .
  Refer [this](https://docs.docker.com/engine/reference/commandline/build/) for additional options.

### Run this container as an independent service:
    $ docker run -d -p 80:80 <image_tag>
  Refer [this](https://docs.docker.com/engine/reference/run/) for additional options.

## TODO
- Update the Dockerfile to use the official mod-pagespeed release tarball once it is available and published.
- Support Alpine Linux version 3.6
