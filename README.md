# Prometheus + Grafana - Examples
This repo contains sample files about Prometheus and Grafana, a very utilized monitoring stack.

## Automated way using docker compose

```bash
docker compose up -d
```

## Manual way
This setups a sample Prometheus docker image/container

```yaml
# build the docker image
docker build -t my-prometheus .
# run the docker container based on the newly generated image
docker run -p 9090:9090 -d --name my-prometheus my-prometheus
```

This setups a sample Prometheus docker image/container

```yaml
docker run -d --name=grafana -p 3000:3000 grafana/grafana-enterprise
```