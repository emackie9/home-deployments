# pi-hole

pi-hole container

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `PIHOLE_TZ`  | No  | Pi-hole timezone. Defaults to `America/Toronto`
| `PIHOLE_WEBPASSWORD`   | Yes | Pi-hole web console password.
| `PIHOLE_WEBPORT`           | No  | Web console port. Defaults to `8080`
