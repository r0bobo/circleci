FROM moby/buildkit:master-rootless

LABEL com.circleci.preserve-entrypoint=true

RUN USER=$(id -u)
USER 0
RUN apk add --no-cache \
    ca-certificates \
    git \
    openssh \
    tar \
    gzip
USER $USER
