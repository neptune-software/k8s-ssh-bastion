FROM ubuntu:24.04
ENV KUBECTL_VERSION=v1.33.0
RUN apt update && apt install --no-install-recommends -y curl ca-certificates telnet openssh-server vim-tiny nmap bind9-host iputils-ping net-tools postgresql-client && apt clean && rm -rf /var/log/* /var/cache/debconf/*-old && update-ca-certificates
RUN set -eux; \
    ARCH=$(dpkg --print-architecture); \
    \
    curl -SL "https://dl.k8s.io/release/${KUBECTL_VERSION}/bin/linux/${ARCH}/kubectl" -o /usr/bin/kubectl; \
    chmod +x /usr/bin/kubectl
