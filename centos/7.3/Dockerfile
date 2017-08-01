FROM eleidan/buildpack-deps-curl:centos-7.3

LABEL maintainer="Oleg Kulyk" \
      description="CentOS 7.3, scm" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/buildpack-deps-scm:centos-7.3" \
      version="2017-08-01"

ENV SERVICE_NAME="buildpack-deps-scm:centos-7.3"

RUN yum -y install \
        bzr \
        git \
        mercurial \
        openssh-client \
        subversion \
        \
        procps \
    && yum clean all
