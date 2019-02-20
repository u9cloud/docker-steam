FROM debian:9-slim
RUN apt-get update && \
    apt-get install -y --no-install-recommends lib32gcc1 && \
    apt-get install -y --reinstall ca-certificates && \
    rm -rf /var/lib/apt/lists/*
ADD https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz /tmp/steamcmd_linux.tar.gz
RUN mkdir /usr/local/steam; \
    tar xvzf /tmp/steamcmd_linux.tar.gz -C /usr/local/steam; \
    rm -rf /tmp/steamcmd_linux.tar.gz
WORKDIR /usr/local/steam
RUN /usr/local/steam/steamcmd.sh +quit
