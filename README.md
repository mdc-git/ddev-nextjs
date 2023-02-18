# ddev-nextjs

Run nextjs in dev mode behind nginx ssl proxy.

Sample Usage:

```
ddev config --auto --omit-containers=db,dba --nodejs-version=16 
mkcert -install
ddev get mdc-git/ddev-nextjs
ddev yarn dev
```
