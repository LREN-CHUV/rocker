
rocker
======

Dockerfiles for different Docker containers of interest to R users.

Work in progress; talk to @eddelbuettel and @cboettig about how to get involved.

Documentation is being added at the [Wiki](https://github.com/rocker-org/rocker/wiki).

## Deferred build actions

We introduce deferred build actions to enable building smaller images that retain a good level of functionality and extensitity. We followed this [blog post](http://blog.dscpl.com.au/2014/12/deferred-build-actions-for-docker-images.html) by Graham Dumpleton.

## Docker user

We setup a default 'docker' user. It is available via runtime flag `--user docker`.
It belongs to 'staff' group, granting it write privileges to /usr/local/lib/R/site.library.
User should also have & own a home directory (for rstudio or linked volumes to work properly). 
