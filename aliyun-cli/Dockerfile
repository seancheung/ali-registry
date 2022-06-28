FROM ubuntu:18.04

ARG BIN_URL='https://aliyuncli.alicdn.com/aliyun-cli-linux-latest-amd64.tgz'
RUN apt-get update && \
    apt-get install -y --no-install-recommends curl tar ca-certificates && \
    curl -L "$BIN_URL" | tar -xz -C /usr/local/bin && \
    apt-get remove -y curl && \
    rm -rf /var/lib/apt/lists/*
