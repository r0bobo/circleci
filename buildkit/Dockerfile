FROM moby/buildkit:master-rootless

RUN USER=$(id -u)
USER 0
RUN apk add --no-cache \
    ca-certificates \
    git \
    openssh \
    tar \
    gzip
USER $USER
