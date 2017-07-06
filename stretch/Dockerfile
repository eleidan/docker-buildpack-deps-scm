FROM eleidan/buildpack-deps-curl:stretch

LABEL maintainer="Oleg Kulyk" \
      description="Debian GNU/Linux stretch, scm" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/buildpack-deps:stretch-scm" \
      version="2017-07-06"

ENV SERVICE_NAME="buildpack-deps:stretch-scm"

RUN apt-get update && apt-get install -y --no-install-recommends \
        bzr \
        git \
        mercurial \
        openssh-client \
        subversion \
        \
        procps \
    && rm -rf /var/lib/apt/lists/*
