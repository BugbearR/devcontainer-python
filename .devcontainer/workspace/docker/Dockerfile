FROM mcr.microsoft.com/devcontainers/python:3.11-bookworm

RUN apt-get update -y \
  && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
  && apt-get autoremove -y \
  && apt-get clean \
  && rm -rf /var/cache/apt/* /var/lib/apt/lists/
