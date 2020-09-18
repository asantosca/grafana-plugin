## Setting up

First let's set up a docker composer file with Grafana and InfluxDB.

* [Grafana](https://github.com/grafana/grafana) - visualization UI for InfluxDB
* [InfluxDB](https://github.com/influxdata/influxdb)

Influxdb is the database that will store the data shown by the plugin.

It is assumed you have Docker/Docker Compose installed and that you know how to use Docker. You can know more about docker compose at https://docs.docker.com/compose/gettingstarted/

## Quick Start

To start the app:

```
docker-compose up -d
```

To stop the app:

1. Run the following command from the root of the cloned repo:
```
docker-compose down
```

Once Grafana is running, open the address 
[http://localhost:3000](http://localhost:3000)

Enter `admin` for the username and `admin` for the password.

Grafana will ask you to change the password.

## What did we do so far?

We have Grafana running and we are able to start and stop it.

We have also InfluxDB installed and configured. We will use it in the next step.
