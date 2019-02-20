FROM u9cloud/steamcmd
ARG STEAM_USERNAME=anonymous
ARG STEAM_PASSWORD
ARG STEAM_APPID
RUN /usr/local/steam/steamcmd.sh +login $STEAM_USERNAME $STEAM_PASSWORD +force_install_dir /opt +app_update $STAEM_APPID +quit
WORKDIR /opt