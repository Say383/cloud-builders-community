FROM debian:11

RUN apt-get update && \
  apt-get install -y ca-certificates curl wget build-essential

ENTRYPOINT ["make"]
