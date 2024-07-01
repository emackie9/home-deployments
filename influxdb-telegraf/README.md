# telegraf

Telegraf for InfluxDB. Use the provided `telegraf.conf` file which contains the following environment variables. Environment variables can be used in configuration files like `token = "$INFLUX_TOKEN"`. Read up on Telegraf configurion [here](https://docs.influxdata.com/telegraf/v1.31/configuration/).

Customize and inject the configuration file into the docker using a method of your choice.

## Docker Compose Environment Variables

| Name                   | Required | Description                                                |
| ---------------------- | -------- | ---------------------------------------------------------- |
| `DOCKER_DAEMON_GRP_ID` | No       | Unix group id for the docker daemon to allow docker access |
| `INFLUX_URL`           | Yes      | Influx DB url                                              |
| `INFLUX_ORGANIZATION`  | Yes      | Influx organization                                        |
| `INFLUX_BUCKET`        | Yes      | Influx bucket                                              |
| `INFLUX_TOKEN`         | Yes      | Influx token which needs write access for the bucket       |
