# ddev-nextjs

## Run nextjs in dev mode behind nginx ssl proxy.

## What does it do?

1. Overwrite `.ddev/nginx_full/nginx-site.conf` to proxy requests to `http://localhost:3000`.
2. Install a `.ddev/docker-compose.network.yaml` to add additional known hosts in the network

## Sample Usage:

```
ddev config --auto --omit-containers=db,dba --nodejs-version=14
mkcert -install
ddev get mdc-git/ddev-nextjs
ddev yarn dev
```
