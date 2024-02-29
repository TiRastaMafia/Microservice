# Запуск контейнера с grafana
```
sudo docker run -d --name=grafana -p 3000:3000 --add-host host.docker.internal=host-gateway grafana/grafana

```


# Запуск контейнера с Prometheus
```
sudo docker run --rm --detach --name my-prometheus --publish 9090:9090 --volume prometheus-vol
ume:/prometheus --volume ./prometheus.yml:/etc/prometheus/prometheus.yml --add-host host.docker.internal=host-gateway prom/prometheus

```

