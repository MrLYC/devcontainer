FROM mcr.microsoft.com/devcontainers/python:0-3.6-buster

ARG DEBIAN_FRONTEND=noninteractive

RUN DEBIAN_FRONTEND=$DEBIAN_FRONTEND \
    && apt-get update \ 
    && apt-get install -y build-essential --no-install-recommends \
    rustc \
    make \
    vim

ARG POETRY_VERSION=1.1.15

RUN echo "done 0" \
    && pip install -U pip \
    && echo "done 1" \
    && pip install poetry==${POETRY_VERSION} \
    && echo "done 2"
