# seedbox

Deluge, Jackett and Flaresolverr routed through a ProtonVPN P2P client. Requires a paid ProtonVPN account and downloads folder mounted through NFS. Also includes TDPS Downloader which will pull TDPS episodes through the VPN.

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `SEEDBOX_PROTONVPN_USERNAME`      | Yes | ProtonVPN username. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_PASSWORD`      | Yes | ProtonVPN password. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_TIER`          | No | ProtonVPN tier, defaults to `2` to support `P2P`. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_SERVER`        | No | ProtonVPN server, defaults to `P2P`. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_EXCLUDE_CIDRS` | Yes | ProtonVPN exclude CIDRs. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_MY_IP`         | Yes | External IP address of host (with no VPN)
| `SEEDBOX_TDPS_LOGIN`              | Yes | Membership login at [TDPS](https://davidpakman.com/)
| `SEEDBOX_TDPS_PASS`               | Yes | Membership password at [TDPS](https://davidpakman.com/)
| `SEEDBOX_TDPS_PATH`               | Yes | Path in container to download shows to
| `SEEDBOX_NFS_CONTENT_HOST`        | Yes | Host of NFS server, ex: `192.168.0.5`
| `SEEDBOX_NFS_CONTENT_PATH`        | Yes | Path on NFS server of mount, ex: `:/mnt/content`
| `SEEDBOX_NFS_DOWNLOADS_HOST`      | Yes | Host of NFS server, ex: `192.168.0.5`
| `SEEDBOX_NFS_DOWNLOADS_PATH`      | Yes | Path on NFS server of mount, ex: `:/mnt/downloads`
| `TZ`                              | No | Defaults to `America/Toronto`