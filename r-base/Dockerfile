## Emacs, make this -*- mode: sh; -*-
 
FROM debian:testing

## This handle reaches Carl and Dirk
MAINTAINER "Carl Boettiger and Dirk Eddelbuettel" rocker-maintainers@eddelbuettel.com

ENV R_BASE_VERSION=3.2.2

COPY setup.sh /usr/local/bin/r-base-docker-setup
COPY install.r /usr/local/bin/install.r
COPY install2.r /usr/local/bin/install2.r
COPY installGithub.r /usr/local/bin/installGithub.r

RUN /usr/local/bin/r-base-docker-setup

CMD ["R"]
