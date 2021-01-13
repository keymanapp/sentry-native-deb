# About this repo

This repo contains the necessary files to create a Debian package for the
[sentry-native](https://github.com/getsentry/sentry-native) library.

It uses git-buildpackage to maintain the source package.

## Branches

The branches used to maintain the package are:

- `upstream` - imported source files from sentry-native
- `main` - merge of `upstream` with the debian package metadata
- `pristine-tar` - contains the original zip file used to import the sources

## Updating to a newer version of `sentry-native`

To update to a newer version of `sentry-native` you can simply run:

```bash
gbp import-orig --uscan
```
