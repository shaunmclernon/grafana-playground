# Grafana playground

Local lab for testing [Grafana] and [Loki] using [docker-compose].

This composition will create the following services:
- [Grafana] - Visualisation UI - http://localhost:3000
- [Loki] - Log store - http://localhost:3001
- [Promtail] - Agent to ship logs to Loki

>NOTE: This is intended for local use only
### Prerequisites

This lab has been setup using:

- [docker] >= 20.10.7
- [docker-compose] >= 1.29.2 

## Quick start

To start the composition:

    docker-compose up -d

To stop the composition:

    docker-compose down

## Data sources

The lab creates a Grafana data source called _Loki_ that's connected to the default _Loki_.

To provision additional data sources, see the Grafana [documentation] and add a config file to `./grafana-provisioning/datasources/` before starting the app.


[Grafana]: https://grafana.com
[Loki]: https://grafana.com/docs/loki/latest/
[docker-compose]: https://docs.docker.com/compose/
[docker]: https://www.docker.com
[Loki]: https://grafana.com/docs/loki/latest/
[Promtail]: https://grafana.com/docs/loki/latest/clients/promtail/
[documentation]: https://grafana.com/docs/grafana/latest/administration/provisioning/#datasources
