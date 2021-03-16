# Kong-Monitoring-With-Prometheus

This simple stack was created for monitoring kong usage using prometheus plugin. Tested localy to monitor grafana as a service. Dashboard template used was available from official grafana dashboard template for kong.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Installing and Running

1. Install Docker & Docker-Compose if it hasn't been installed on your machine and run it.\
[Docker Install](https://docs.docker.com/get-docker/) & [Docker-Compose Install](https://docs.docker.com/compose/install/)

2. Clone this repository into your machine.
```
$ git clone https://github.com/revawiki/Kong-Monitoring-With-Prometheus.git
```

3. Edit docker-compose.yml in grafana folder, change the IP address to your current IP address.
```
$ - GF_SERVER_ROOT_URL=http://192.168.1.1:8000/grafana-test
```

4. Create external network for docker container used in this stack.
```
$ docker network create kong-net
```

5. In each folder, run the docker-compose start script.
```
$ ./up.sh
```

### Konga and Grafana Config

1. Access Konga web admin (http://locahost:9000)

2. Create Grafana as a service with Host IP (192.168.1.1 { your local address }) and Port (3000). Add route with Path (grafana-test),

3. If succeed, grafana can be accessed in (http://<span></span>{ your Local address }:8000/grafana-test)

4. Back to Konga, access Plugin menu. Add global plugin, in Analitycs & Monitoring categories choose Prometheus. Left empty by default and add plugin.

5. In Grafana, add Prometheus as datasource. Aliases used was (http://<span></span>kongmon-prometheus:9090)

6. Import dashboard template using official Kong for Grafana dashboard (linked below)


## Built With

* [Grafana](http://www.grafana.com) for Data Visualization.
* [Docker](https://www.docker.com) for Virtualization.
* [Prometheus](https://prometheus.io/) for Scraper and Datasource.
* [Kong](https://konghq.com/) for API Gateway.
* [Konga](https://github.com/pantsel/konga) for Kong UI.

## Credits

* [Official Dashboard Template](https://grafana.com/grafana/dashboards/7424) by KongHQ

##### Question/Inquiries
If you have any question regarding the repo, feel free to e-mail me at reva.wiki@gmail.com. Thank you.
