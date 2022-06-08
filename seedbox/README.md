# seedbox

Deluge, Jackett and Flaresolverr routed through a ProtonVPN P2P client. Requires a paid ProtonVPN account and downloads folder mounted through NFS. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `SEEDBOX_PROTONVPN_USERNAME`      | Yes | ProtonVPN username. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_PASSWORD`      | Yes | ProtonVPN password. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_TIER`          | No | ProtonVPN tier, defaults to `2` to support `P2P`. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_SERVER`        | No | ProtonVPN server, defaults to `P2P`. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_EXCLUDE_CIDRS` | Yes | ProtonVPN exclude CIDRs. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_MY_IP`         | Yes | External IP address of host (with no VPN)
| `SEEDBOX_NFS_DOWNLOADS_HOST`      | Yes | Host of NFS server, ex: `192.168.0.5`
| `SEEDBOX_NFS_DOWNLOADS_PATH`      | Yes | Path on NFS server of mount, ex: `:/mnt/downloads`
| `SEEDBOX_DOWNLOADS_VOLUME`        | No | Name of volume where to store downloads. Defaults to `content_downloads`
| `SEEDBOX_NETWORK`                 | No | Network on Docker engine to deploy to. Defaults to `proxy_network`
| `TZ`                              | No | Defaults to `America/Toronto`
