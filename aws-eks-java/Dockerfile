FROM amazonlinux:latest

RUN yum update -y && yum install -y \
  ca-certificates \
  groff \
  less \
  curl \
  wget \
  zip \
  openssl \
  git \
  ca-certificates \
  bash \
  jq \
  unzip \
  tar \
  python3

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && unzip awscliv2.zip && ./aws/install && rm -rf aws/*

RUN amazon-linux-extras install java-openjdk11

ENTRYPOINT ["/bin/bash"]
