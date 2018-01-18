# KrakenD CE

[![Build Status](https://travis-ci.org/devopsfaith/krakend-ce.svg?branch=master)](https://travis-ci.org/devopsfaith/krakend-ce)

KrakenD Community Edition is the Open Sourced binary for the [KrakenD](http://www.krakend.io).

## Documentation

Full, comprehensive documentation is viewable on the KrakenD website:

http://www.krakend.io/docs/overview/introduction/

## Build Requirements

- golang 1.9
- `dep`

## Build
```
	make prepare
	make
```

## Building with docker

If you don't have or dont want to install `go` you can build it using the golang docker container.
```
make docker_build
```

## FPM
You can setup your own fpm docker image to run setting `DOCKER_FPM` on the `Makefike`.


## Using the generated packages
The package will create a krakend user to run the service and will configure the service to run under systemd.

## Linux Distributions
* just any Linux (using the `tar.gz`)
* ubuntu 14.04, 16.04 (should run un 17.04/10 too)
* Debian 7, 8, 9
* centos 6, 7

```
deb: ubuntu debian
rpm: el6 el7

ubuntu: ubuntu-trusty ubuntu-xenial
debian: debian-wheezy debian-jessie debian-stretch
```