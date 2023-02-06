# Monitoring with Prometheus and Grafana

In today's world, metrics collection is mandatory in order to effective monitoring. To do so, it is quite common to use [Prometheus](https://prometheus.io/) and [Grafana](https://grafana.com/). 

[Prometheus](https://prometheus.io/) is a powerful metrics collection and alerting system, and [Grafana](https://grafana.com/) is one of the best visualization tools which can be used with Prometheus. 

We can create a dashboard with multiple charts together in Grafana. 

## Run the stack

In order to tun Prometheus and Grafana, run the following command

```bash
$ docker-compose up -d
```
> By default, in the configuration folder, the file prometheus.yml adds a new job that will be pooling every 5 seconds to http://localhost/actuator/prometheus. Change that configuration according to your needs.

## Prometheus

Open a browser and point at http://localhost:9090/ for Prometheus.

## Grafana

Step by step initial instructions:

1. Open a browser and point at http://localhost:3000/ for Grafana.
2. Use admin/admin as initial username and password.
3. Set a new password when prompted.
4. Add a new Data Source, choosing type Prometheus.
5. Set up the datasource, using http://prometheus:9090 as URL.
6. Save and Test the new Data Source.
7. In the left toolbar, click on the button 'Explore'. With the selector metrics, play with some metrics.
8. In the left toolbar, click on the button 'Dashboard', to create your own dashboards.
