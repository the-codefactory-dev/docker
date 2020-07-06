FROM python:3.7-ubuntu

RUN apk --no-cache add \
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
  jq

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

RUN unzip awscliv2.zip

RUN ./aws/install
