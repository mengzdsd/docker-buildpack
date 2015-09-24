# This is a Dockerfile to build a base ubuntu image
FROM buildpack-deps:trusty-curl
MAINTAINER Mengz You <mengz.you@outlook.com>

# Environments
ENV OS_NAME "Ubuntu"
ENV OS_VERSION_ID "14.04"
ENV OS_VERSION "14.04.3 LTS, Trusty Tahr"
ENV DEBIAN_FRONTEND "noninteractive"

# Update and install tool packages
RUN apt-get update \
  && apt-get install -y build-essential apt-utils --no-install-recommends \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*
