# renovate-repro-major-not-updated

## Summary

The reproduction repository has dependency to `github.com/google/go-github/v44 v44.0.0`.
New versions `v44.1.0` and `v45.2.0` are available.

### Expected behavior

Major version update PR (`Update module github.com/google/go-github/v44 to v45`) and minor version update PR (`Update module github.com/google/go-github/v44 to v44.1.0`) is created.

### Actual behavior

Major version update PR of Go module is not created.
Only minor version update PR (`Update module github.com/google/go-github/v44 to v44.1.0`) is created.


## Reproduce on self-hosted Renovate

Setting `GOPROXY` to the self-hosted Renovate reproduces the problem locally.

```shell
cd .renovate
docker-compose up
```
