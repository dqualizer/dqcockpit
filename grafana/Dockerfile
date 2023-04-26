FROM grafana/grafana

USER root
WORKDIR /tmp

ENV GF_PATHS_PROVISIONING=/usr/share/grafana/custom/
ENV GF_SECURITY_ADMIN_PASSWORD=demo
ENV GF_USERS_DEFAULT_THEME=light

COPY provisioning /usr/share/grafana/custom/

###
# Future Options: Installing further grafana panels
###
USER grafana
RUN grafana-cli plugins install yesoreyeram-boomtheme-panel
# 		grafana-cli plugins install grafana-polystat-panel && \
# 		grafana-cli plugins install novatec-sdg-panel