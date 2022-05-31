# tickstack

InfluxDB and Telegraf. Environment variables can be used in configuration files like `token = "$INFLUX_TOKEN"`. Read up on Telegraf configurion [here](https://docs.influxdata.com/telegraf/v1.22/configuration/).

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `INFLUX_ORGANIZATION` | Yes | Setup InfluxDB first then provide organization value here
| `INFLUX_BUCKET`       | Yes | Setup InfluxDB first then provide bucket value here
| `INFLUX_TOKEN`        | Yes | Setup InfluxDB first then provide token value here