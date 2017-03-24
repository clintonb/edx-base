# docker build -t clintonb/edx-base:alpine - < alpine/Dockerfile

FROM python:3.5-alpine
ENV PYTHONUNBUFFERED 1

# NOTE: We need mariadb-dev for MySQL since there is no libmysqlclient-dev for Alpine.
# See https://bugs.alpinelinux.org/issues/4768 for details.
RUN apk add --update \
    build-base \
    gettext \
    libffi-dev \
    libjpeg-turbo-dev \
    libmemcached-dev \
    mariadb-dev \
    nodejs \
    zlib-dev
