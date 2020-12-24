FROM ubuntu:latest as check_eol

RUN  apt update && apt install -y  git

WORKDIR /app
COPY entrypoint.sh /

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/bin/bash", "/entrypoint.sh"]

