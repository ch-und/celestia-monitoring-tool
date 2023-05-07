# celestia-monitoring-tool

After writing [The Blockspace Race — Perform my Celestia light node](https://medium.com/@batuoc90/the-blockspace-race-perform-my-celestia-light-node-1f70c24ec866) article, I consulted and rebuilt more comprehensive dashboards. In addition, I integrated `alertmanager` to help users receive alerts about node status via Telegram. Moreover, I put everything into a docker project, so that everyone can deploy it to their node easily.

## Includes

### Containers
- [grafana sever](https://hub.docker.com/r/grafana/grafana)
- [node_exporter](https://hub.docker.com/r/prom/node-exporter)
- [prometheus](https://hub.docker.com/r/prom/prometheus)
- [alertmanager](https://hub.docker.com/r/prom/alertmanager)


### Dashboards
- [Node Exporter Full dashboard](https://github.com/rfrail3/grafana-dashboards)
- [Node Exporter for Prometheus Dashboard EN](https://github.com/starsliao/Prometheus/tree/master/node_exporter)

### Alerts

- Server down
- Out of memory (<10%)
- Out of disk space (<10%)
- Out of disk space within 24h
- High CPU load (>85%)

## Installation

### Clone this repo
```
cd
git clone https://github.com/ch-und/celestia-monitoring-tool.git
```

### Install docker
You need docker to deploy this project. So, you can run this command:
```
bash $HOME/celestia-monitoring-tool/utils/install_docker.sh
```
