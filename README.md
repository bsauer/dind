# dind
_dind_ is like docker:dind but lets you pass additional command line flags using *DOCKER_OPTS* Environment Variable.

[![Build Status Widget]][Build Status] [![Code Climate Widget]][Code Climate] [![MicroBadger Image Widget]][MicroBadger URL]

[Build Status]: https://travis-ci.org/bsauer/dind
[Build Status Widget]: https://travis-ci.org/bsauer/dind.svg?branch=master
[Code Climate]: https://codeclimate.com/github/bsauer/dind
[Code Climate Widget]: https://codeclimate.com/github/bsauer/dind/badges/gpa.svg
[MicroBadger URL]: http://microbadger.com/#/images/bsauer/dind
[MicroBadger Image Widget]: https://images.microbadger.com/badges/image/bsauer/dind.svg

## Example

    docker run --privileged -e "DOCKER_OPTS=--storage-driver=overlay" bsauer/dind

## Docker Hub
Automated build is available at the [Docker Hub](https://hub.docker.com/r/bsauer/dind).
