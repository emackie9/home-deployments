# plex

Plex server.

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `PLEXSTACK_NFS_CONTENT_HOST`  | Yes | Host of NFS server containing content, ex: `192.168.0.4`
| `PLEXSTACK_NFS_CONTENT_PATH`  | Yes | Path on NFS server of mount, ex: `:/mnt/content`
| `PLEXSTACK_CONTENT_DIR`       | No | Directory inside plex which should contain content (useful for migrations). Defaults to `/content`
| `PLEXSTACK_CONTENT_VOLUME`    | No | Name of volume where to read content. Defaults to `content`
| `TZ`  | No  | Defaults to `America/Toronto`