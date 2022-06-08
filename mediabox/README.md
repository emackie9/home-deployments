# mediabox

Lidarr, Radarr, Sonarr and seperate Radarr and Sonarr instance exclusively for 4K content. Downloads and content folders are mounted through NFS. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `MEDIABOX_NETWORK`            | No | Network on Docker engine to deploy to. Defaults to `proxy_network
| `MEDIABOX_CONTENT_VOLUME`     | No | Name of volume where to read content. Defaults to `content`
| `MEDIABOX_DOWNLOADS_VOLUME`   | No | Name of volume where to store downloads. Defaults to `content_downloads`
| `TZ`                          | No | Defaults to `America/Toronto`