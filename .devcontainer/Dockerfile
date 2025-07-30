FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN --mount=type=cache,target=/var/cache/apt \
    apt-get update && \
    apt-get install -y \
    # dev tools
    git \
    # build tools
    build-essential \
    cmake \
    gdb