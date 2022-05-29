# nextcloud

Nextcloud with Redis, MariaDB and webcron job at 300 second intervals. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `NEXTCLOUD_TRUST_PROXIES`     | Yes | Trusted proxy server ex: `192.168.0.0/24`
| `NEXTCLOUD_HOST_PORT`         | No  | Nextcloud web port to expose, defaults to `8080`
| `NEXTCLOUD_WEBCRON_URL`       | Yes | Nextcloud webcron url should end in `cron.php`
| `NEXTCLOUD_WEBCRON_INTERVAL`  | No  | Nextcloud webcron interval in seconds, defaults to `300`