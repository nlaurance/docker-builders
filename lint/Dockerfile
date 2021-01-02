ARG PY_VERSION=3.9

FROM python:${PY_VERSION} as base
MAINTAINER nicolas.laurance@gmail.com

RUN pip install --upgrade pip pip-tools
COPY requirements.in .
RUN pip-compile requirements.in
RUN pip install -r requirements.txt

# PY_VERSION=3.9-slim; docker build --build-arg PY_VERSION=${PY_VERSION} --tag nlaurance/lint:${PY_VERSION} .

