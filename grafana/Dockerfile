FROM grafana/grafana:9.2.15-ubuntu

USER root
WORKDIR /tmp

ENV GF_PATHS_PROVISIONING=/usr/share/grafana/custom/
ENV GF_SECURITY_ADMIN_PASSWORD=demo

COPY provisioning /usr/share/grafana/custom/

###
# Future Options: Installing further grafana panels
###
# USER grafana
# RUN grafana-cli plugins install grafana-polystat-panel && \
# 		grafana-cli plugins install novatec-sdg-panel