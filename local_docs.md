# Local_doc

> 来自Local_doc的md

## Docker操作

docker build . -t ghcr.io/yingchaoorg/local_docs-laravel-cn-docs:10.x

docker  stop local_docs-laravel-10.x-cn-docs
docker  rm local_docs-laravel-10.x-cn-docs

docker run -it  --name local_docs-laravel-10.x-cn-docs -p 34809:80 -d --rm -v ./:/usr/share/nginx/html ghcr.io/yingchaoorg/local_docs-laravel-cn-docs:10.x

docker  exec -it  local_docs-laravel-10.x-cn-docs  bash

## bash脚本

```bash

#!/bin/bash

Header always set Content-Security-Policy "script-src 'self'"
add_header Content-Security-Policy "script-src 'self'";

<meta http-equiv="content-security-policy" content="策略集">


```