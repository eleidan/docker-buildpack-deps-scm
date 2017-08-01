FROM eleidan/buildpack-deps-curl:xenial

LABEL maintainer="Oleg Kulyk" \
      description="Ubuntu 16.04 xenial, scm" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/buildpack-deps-scm:xenial" \
      version="2017-07-09"

ENV SERVICE_NAME="buildpack-deps-scm:xenial"

RUN apt-get update && apt-get install -y --no-install-recommends \
        bzr \
        git \
        mercurial \
        openssh-client \
        subversion \
        \
        procps \
    && rm -rf /var/lib/apt/lists/*
