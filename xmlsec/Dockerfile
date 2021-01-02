ARG PY_VERSION=3.8-slim

FROM python:${PY_VERSION} as base
MAINTAINER nicolas.laurance@gmail.com

RUN apt update && apt install -y \
    libxml2-dev libxmlsec1-dev libxmlsec1-openssl \
    && pip install --upgrade pip xmlsec

# docker build -t nlaurance/pyxmlsec:3.8 .