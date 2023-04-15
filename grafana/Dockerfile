FROM grafana/grafana:9.4.0


#RUN apt-get update && apt-get install -y curl gettext-base && rm -rf /var/lib/apt/lists/*
RUN rm -rf /var/lib/apt/lists/*

WORKDIR /etc/grafana
COPY datasources ./datasources

WORKDIR /app
COPY entrypoint.sh ./
#RUN chmod u+x entrypoint.sh

#ENTRYPOINT ["/app/entrypoint.sh"]
ENTRYPOINT ["/entrypoint.sh"]