FROM u9cloud/steamcmd
RUN /usr/local/steam/steamcmd.sh +login $STEAM_USERNAME $STEAM_PASSWORD +force_install_dir /opt +app_update $STAEM_APPID +quit
WORKDIR /opt