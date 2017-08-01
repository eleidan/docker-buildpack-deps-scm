FROM eleidan/buildpack-deps-curl:centos-6.6

LABEL maintainer="Oleg Kulyk" \
      description="CentOS 6.6, scm" \
      run="docker run -it --rm -v $(pwd):/home/phantom/app eleidan/buildpack-deps-scm:centos-6.6" \
      version="2017-08-01"

ENV SERVICE_NAME="buildpack-deps-scm:centos-6.6"

RUN yum install -y yum-plugin-ovl \
    && yum -y install \
        bzr \
        git \
        mercurial \
        openssh-client \
        subversion \
        \
        procps \
    && yum clean all
