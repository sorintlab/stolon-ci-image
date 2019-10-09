# Stolon CI image

This is the stolon ci image use by the stolon project to execute its tests inside our Agola CI/CD (https://agola.io) instance.

### Build images for any required postgres version

```
VERSION=v0.1.0; for i in 9.5 9.6 10 11 12; do make PGVERSION=$i TAG=sorintlab/stolon-ci-image:$VERSION-pg$i; done
```
