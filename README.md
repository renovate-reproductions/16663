# renovate-repro-major-not-updated

## Summary

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
