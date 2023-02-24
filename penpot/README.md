# penpot

Penpot stack.

## Docker Compose Environment Variables

| Name | Required | Description
|---|---|---
| `PENPOT_FRONTEND_FLAGS`       | No  | Flags to pass to Penpot frontend. See more [here](https://help.penpot.app/technical-guide/configuration/#advanced-configuration). Defaults to `enable-registration enable-login-with-password`
| `PENPOT_BACKEND_FLAGS`        | No  | Flags to pass to Penpot backend. See more [here](https://help.penpot.app/technical-guide/configuration/#advanced-configuration). Defaults to `enable-registration enable-login-with-password disable-email-verification enable-smtp enable-prepl-server disable-secure-session-cookies`
| `PENPOT_SECRET_KEY`           | Yes | Serves as a master key from which other keys for subsystems (eg http sessions) are derived. Generate with `python3 -c "import secrets; print(secrets.token_urlsafe(64))"`
| `PENPOT_PUBLIC_URI`           | No  | Public URI. Defaults to `http://penpot.localhost`
| `PENPOT_HOST`                 | No  | Public URI. Defaults to `penpot.localhost`
| `PENPOT_TELEMETRY_ENABLED`    | No  | Telemetry. When enabled, a periodical process will send anonymous data about this instance. Defaults to `false`
| `PENPOT_SMTP_HOST`            | Yes | SMTP server host. Emails are used to confirm user registrations & invitations. 
| `PENPOT_SMTP_PORT`            | No  | SMTP server port. Defaults to `1025`
| `PENPOT_SMTP_USERNAME`        | Yes | SMTP server username. 
| `PENPOT_SMTP_PASSWORD`        | Yes | SMTP server password. 
| `PENPOT_SMTP_TLS`             | No  | Defaults to `false`
| `PENPOT_SMTP_SSL`             | No  | Defaults to `false`
| `PENPOT_SMTP_DEFAULT_FROM`    | Yes | SMTP server from address. 
| `PENPOT_SMTP_DEFAULT_REPLY_TO`| Yes | SMTP server reply to address. 