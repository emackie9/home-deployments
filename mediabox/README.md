# mediabox

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `MEDIABOX_NFS_CONTENT_HOST`   | Yes | Host of NFS server containing content, ex: `192.168.0.4`
| `MEDIABOX_NFS_CONTENT_PATH`   | Yes | Path on NFS server of mount, ex: `:/mnt/content`
| `MEDIABOX_NFS_DOWNLOADS_HOST` | Yes | Host of NFS server containing downloads, ex: `192.168.0.4`
| `MEDIABOX_NFS_DOWNLOADS_PATH` | Yes | Path on NFS server of mount, ex: `:/mnt/downloads`
| `TZ`                          | No | Defaults to `America/Toronto`