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

RUN curl -O https://bootstrap.pypa.io/get-pip.py && python3 get-pip.py --user && rm get-pip.py

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && unzip awscliv2.zip && ./aws/install && rm -rf aws/*

ENTRYPOINT ["/bin/bash"]
