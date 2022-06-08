# mediabox

Lidarr, Radarr, Sonarr and seperate Radarr and Sonarr instance exclusively for 4K content. Downloads and content folders are mounted through NFS. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `MEDIABOX_NFS_CONTENT_HOST`   | Yes | Host of NFS server containing content, ex: `192.168.0.4`
| `MEDIABOX_NFS_CONTENT_PATH`   | Yes | Path on NFS server of mount, ex: `:/mnt/content`
| `MEDIABOX_NFS_DOWNLOADS_HOST` | Yes | Host of NFS server containing downloads, ex: `192.168.0.4`
| `MEDIABOX_NFS_DOWNLOADS_PATH` | Yes | Path on NFS server of mount, ex: `:/mnt/downloads`
| `MEDIABOX_NETWORK`           | No | Network on Docker engine to deploy to. Defaults to `proxy_network`
| `TZ`                          | No | Defaults to `America/Toronto`