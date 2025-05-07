FROM ubuntu:24.04
RUN apt update && apt install --no-install-recommends -y curl telnet openssh-server vim-tiny nmap bind9-host iputils-ping net-tools postgresql-client && apt clean && rm -rf /var/log/* /var/cache/debconf/*-old
