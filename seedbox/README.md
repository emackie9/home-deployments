# seedbox

Deluge, Jackett and Flaresolverr routed through a ProtonVPN P2P client. Requires a paid ProtonVPN account and downloads folder mounted through NFS. 

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `SEEDBOX_QBITTORENT_VOLUME`       | No  | qBittorrent local volume to use for config. Defaults to `seedbox_qbittorrent`
| `SEEDBOX_QBITTORRENT_VERSION`     | No  | qBittorrent image tag to pull. Defaults to `latest`
| `SEEDBOX_PROTONVPN_VERSION`       | No  | ProtonVPN container version, defaults to `7.2.0`. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_SERVER`        | Yes | ProtonVPN server to connect to. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_KEY`           | Yes | ProtonVPN Wireguard Private key. See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_PROTONVPN_KILL_SWITCH`   | No  | ProtonVPN enable kill-switch (experimental and can cause issues), defaults to `0` (off). See [ProtonVPN](https://github.com/tprasadtp/protonvpn-docker)
| `SEEDBOX_NFS_DOWNLOADS_HOST`      | Yes | Host of NFS server, ex: `192.168.0.5`
| `SEEDBOX_NFS_DOWNLOADS_PATH`      | Yes | Path on NFS server of mount, ex: `:/mnt/downloads`
| `SEEDBOX_DOWNLOADS_VOLUME`        | No  | Name of volume where to store downloads. Defaults to `content_downloads`
| `SEEDBOX_NETWORK`                 | No  | Network on Docker engine to deploy to. Defaults to `proxy_network`
| `SEEDBOX_TZ`                      | No  | Defaults to `America/Toronto`
