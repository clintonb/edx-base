# docker build -t clintonb/edx-base:python-2.7-slim - < python/2.7/slim/Dockerfile

FROM python:2.7-slim
ENV PYTHONUNBUFFERED 1

RUN apt-get update && \
    apt-get install -y curl && \
    curl -sL https://deb.nodesource.com/setup_6.x | bash - && \
    apt-get install -y \
        build-essential \
        gettext \
        git \
        libffi-dev \
        libjpeg-dev \
        libmemcached-dev \
        libmysqlclient-dev \
        libpng12-dev \
        libssl-dev \
        nodejs
