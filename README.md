# Grafana playground

Local lab for testing [Grafana] and [Loki] using [docker-compose]

>NOTE: This is intended for local use only

## Prerequisites

This lab has been setup using:

- [docker] >= 20.10.7
- [docker-compose] >= 1.29.2 

## Usage

    docker-compose up -d

This composition will create the following containers
- [Grafana] (visualize metrics) http://localhost:3000
- [Loki] (log store) http://localhost:3001
- [Promtail] (agent to ship logs to Loki)

Navigate to http://localhost:3000 and login with user creds in config file.


[Grafana]: https://grafana.com
[Loki]: https://grafana.com/docs/loki/latest/
[docker-compose]: https://docs.docker.com/compose/
[docker]: https://www.docker.com
[Loki]: https://grafana.com/docs/loki/latest/
[Promtail]: https://grafana.com/docs/loki/latest/clients/promtail/
