# Kong-Monitoring-With-Prometheus

This simple stack was created for monitoring kong usage using prometheus plugin. Tested localy to monitor grafana as a service. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Installing and Running

1. Install Docker & Docker-Compose if it hasn't been installed on your machine and run it.\
[Docker Install](https://docs.docker.com/get-docker/) & [Docker-Compose Install](https://docs.docker.com/compose/install/)

2. Clone this repository into your machine.
```
$ git clone https://github.com/revawiki/Basic-TIG-Stack-For-Mongo-Monitoring.git
```

3. Go to the cloned directory, and execute this bashfile (with Docker running in the background).
```
$ ./up.sh
```

4. With your browser, access grafana via (http://localhost:3000), login with default username:password (admin:changeme)

5. Dashboard template is available for download from Grafana Dashboard Collection Site (linked below).


## Built With

* [Grafana](http://www.grafana.com) for Data visualization.
* [Mongo](https://www.mongodb.com/) for DBS.
* [Docker](https://www.docker.com) for Virtualization.

## Credits

* [Dashboard Template](https://grafana.com/grafana/dashboards/2583) by Saada

##### Question/Inquiries
If you have any question regarding the repo, feel free to e-mail me at reva.wiki@gmail.com. Thank you.
