# docker-fpm

Use it from the [Docker Hub](http://hub.docker.com/r/devopsfaith/fpm).

## Deb packages

Uses Ubuntu Xenial,

```
docker build -t fpm:deb deb
```

## RPM packages

Uses CentOS 7, if you want another rpm-flavored distro, change the `FROM` in the `Dockerfile`.

```
docker build -t fpm:rpm fpm
```

## Custom Linux distributions

For another deb-flavored distro, change the `FROM` in the `deb/Dockerfile`.
For another rpm-flavored distro, change the `FROM` in the `rpm/Dockerfile`.
