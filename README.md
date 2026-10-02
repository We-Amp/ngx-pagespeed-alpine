# ngx-pagespeed-alpine

> **This repository is archived.** It held the Alpine Linux Dockerfiles for the
> Google-era ngx_pagespeed images, last updated in 2018 (the Docker Hub tags stop
> at 1.13.35.2). PageSpeed for nginx is maintained again as the nginx module of
> [mod_pagespeed 2.1](https://github.com/We-Amp/mod_pagespeed), which is open
> source under the Apache License 2.0.

## Where to go

| | |
|---|---|
| **Run PageSpeed for nginx in a container** | [Install with Docker →](https://modpagespeed.com/docs/installation-docker/) — `ghcr.io/we-amp/pagespeed-nginx`, `pagespeed-combined`, `pagespeed-worker` (signed images, amd64 + arm64) |
| **Read or build the nginx module source** | [`pagespeed/nginx/` in We-Amp/mod_pagespeed →](https://github.com/We-Amp/mod_pagespeed/tree/master/pagespeed/nginx) |
| **Install the prebuilt, signed module** (Debian, Ubuntu, EL9 — amd64 + arm64) | [Install guide →](https://github.com/We-Amp/mod_pagespeed/blob/master/docs/install-nginx.md) |
| **Build against your own nginx** | [ngxpagespeed.com/install/from-source →](https://ngxpagespeed.com/install/from-source/) |
| **Report a bug or ask a question** | [Open an issue →](https://github.com/We-Amp/mod_pagespeed/issues) |

No Alpine (musl) build of the maintained module is published. The container
images above are the supported container path.

## About the files in this repository

The `stable/` tree keeps the original Alpine Dockerfiles for reference. They
build the archived Google-era module (1.13.35.2) against nginx 1.14/1.15 and
have not been updated since 2018. The upstream copies moved to
[apache/incubator-pagespeed-ngx/docker](https://github.com/apache/incubator-pagespeed-ngx/tree/master/docker)
at the time; both are unmaintained. Do not use them for a new deployment.

The original images were published to
[Docker Hub as `pagespeed/nginx-pagespeed`](https://hub.docker.com/r/pagespeed/nginx-pagespeed).
