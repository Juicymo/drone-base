# Juicymo Drone CI base image

We use this image at [Juicymo](http://www.juicymo.cz) when we derive new more specialized Drone CI images from it (like [juicymo/drone-ruby]).

## Installation

Compiled Docker image can be pulled from: TBD

## About

This is a base image for [drone](https://github.com/drone/drone) based on the [phusion/baseimage](https://github.com/phusion/baseimage-docker), inspired by [wingrunr21/drone-base](https://github.com/wingrunr21/drone-base).

This image currently installs:

* wget, build-essential, git, socat, imagemagick (and associated dev packages)
* PostgreSQL client and MySQL client (and associated dev packages)
* sqlite dev packages
* xvfb and phantomjs
* nodejs
* ruby-install and chruby
* ruby 2.2.2

More ruby versions or other software can be added by use of additional images derived from this one instead (like [juicymo/drone-ruby](https://github.com/Juicymo/drone-ruby) for Ruby CI).