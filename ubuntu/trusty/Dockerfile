FROM eleidan/buildpack-deps-curl:trusty

LABEL maintainer="Oleg Kulyk" \
      description="Ubuntu 14.04 trusty, scm" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/buildpack-deps-scm:trusty" \
      version="2017-07-09"

ENV SERVICE_NAME="buildpack-deps-scm:trusty"

RUN apt-get update && apt-get install -y --no-install-recommends \
        bzr \
        git \
        mercurial \
        openssh-client \
        subversion \
        \
        procps \
    && rm -rf /var/lib/apt/lists/*
