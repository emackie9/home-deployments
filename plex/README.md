# plex

Plex server.

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `PLEXSTACK_CONTENT_DIR`       | No | Directory inside plex which should contain content (useful for migrations). Defaults to `/content`
| `PLEXSTACK_CONTENT_VOLUME`    | No | Name of volume where to read content. Defaults to `content`
| `TZ`  | No  | Defaults to `America/Toronto`