# Apt-Cacher NG

Apt-Cacher NG is a caching HTTP proxy intended for use with download clients of system distribution's package managers. Supports Debian/Ubuntu (good), ArchLinux/OpenSUSE/Cygwin (basic). Target use case: alternative to local distro mirror in small LANs.

> [https://alioth.debian.org/projects/apt-cacher-ng/](https://alioth.debian.org/projects/apt-cacher-ng/)

## Supported tags and respective `Dockerfile` links

[![](https://images.microbadger.com/badges/image/sashgorokhov/docker-apt-cacher-ng.svg)](https://microbadger.com/images/sashgorokhov/docker-apt-cacher-ng "Get your own image badge on microbadger.com")
-	`latest` [(*Dockerfile*)](https://github.com/sashgorokhov/docker-teamcity-agent/blob/master/Dockerfile)

## How to use this image

```console
docker run --name apt-cacher-ng -p 3142:3142 -d sashgorokhov/docker-apt-cacher-ng
```

The default port that apt-cacher-ng listens is `3142`.

This image is very simple and contains no extra logic for managing custom bind port or apt-cacher-ng settings, and this suits my requirements. Feel free to extend this image and add something useful. 
