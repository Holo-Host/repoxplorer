FROM 028550861172.dkr.ecr.us-west-2.amazonaws.com/devops/gitcommithistory:latest
LABEL maintainer="mamading.ceesay@holo.host"

ARG version=1.5.1-holo2-dec-2020

COPY ./.holo/holo-host.yaml /etc/repoxplorer/defs
COPY ./.holo/holochain.yaml /etc/repoxplorer/defs
COPY ./.holo/repoxplorer-git-credentials-helper /usr/local/bin/repoxplorer-git-credentials-helper

EXPOSE 51000

CMD ["supervisord", "-n", "-c", "/etc/supervisord.conf"]

