# plex

Plex server.

## Docker Compose Environment Variables

| Name                    | Required | Description                                                                                                                                                                   |
| ----------------------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `PLEX_ADVERTISE_IP`     | Yes      | Defines the additional IPs on which the server may be be found. For example: `http://10.1.1.23:32400`. See [plexinc/pms-docker](https://hub.docker.com/r/plexinc/pms-docker/) |
| `PLEX_CONFIG`           | No       | Name of volume where to read configurations. Needs to be created beforehand. Defaults to `plex_config`                                                                        |
| `PLEX_CONTENT`          | No       | Name of volume where to read content. Needs to be created beforehand. Defaults to `content`                                                                                   |
| `PLEX_CONTENT_INTERNAL` | No       | Directory inside plex which should contain content (useful for migrations). Defaults to `/content`                                                                            |
| `PLEX_NETWORK`          | No       | Plex network to use. Needs to be created beforehand. Defaults to `plex_network`                                                                                               |
| `PLEX_TAG`              | No       | Plex image tag to pull. Defaults to `latest`                                                                                                                                  |
| `PLEX_TZ`               | No       | Defaults to `America/Toronto`                                                                                                                                                 |
