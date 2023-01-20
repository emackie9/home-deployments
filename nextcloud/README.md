# nextcloud

Nextcloud with Redis, MariaDB and webcron job at 300 second intervals. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `NEXTCLOUD_TRUSTED_DOMAINS`   | Yes | Optional space-separated list of domains
| `NEXTCLOUD_TRUSTED_PROXIES`   | Yes | Trusted proxy server ex: `192.168.0.0/24`
| `NEXTCLOUD_CLI_URL`           | Yes | Set the cli url of the proxy (e.g. https://mydnsname.example.com)
| `NEXTCLOUD_HOST`              | Yes | Set the hostname of the proxy. Can also specify a port.
| `NEXTCLOUD_PROTOCOL`          | Yes | Set the protocol of the proxy, http or https.
| `NEXTCLOUD_WEBCRON_URL`       | Yes | Nextcloud webcron url should end in `cron.php`
| `NEXTCLOUD_WEBCRON_INTERVAL`  | No  | Nextcloud webcron interval in seconds, defaults to `300`
| `NEXTCLOUD_NETWORK`           | No  | Network on Docker engine to deploy to. Defaults to `proxy_network`
| `NEXTCLOUD_AWS_VOLUME`        | No  | Docker volume for AWS credentials. Defaults to `aws_credentials`
| `NEXTCLOUD_REDIS_TAG`         | No  | Tag for redis image. Defaults to `7-alpine`