# outline

Outline stack, see their [GitHub](https://github.com/outline/outline) page for more details.

## Docker Compose Environment Variables

See [.env.sample](https://github.com/outline/outline/blob/main/.env.sample) for details.

| Name                       | Required | Description                                         |
| -------------------------- | -------- | --------------------------------------------------- |
| `OUTLINE_NETWORK`          | No       | Outline network to use. Defaults to `proxy_network` |
| `OUTLINE_VERSION`          | No       | Outline image tag to use. Defaults to `0.74.0`      |
| `OUTLINE_SECRET`           | Yes      |                                                     |
| `OUTLINE_UTILS_SECRET`     | Yes      |                                                     |
| `OUTLINE_URL`              | Yes      | Public URI.                                         |
| `OUTLINE_PORT`             | No       | Defaults to `3000`                                  |
| `OUTLINE_SMTP_HOST`        | Yes      | SMTP server host.                                   |
| `OUTLINE_SMTP_PORT`        | No       | SMTP server port. Defaults to `1025`                |
| `OUTLINE_SMTP_USERNAME`    | Yes      | SMTP server username.                               |
| `OUTLINE_SMTP_PASSWORD`    | Yes      | SMTP server password.                               |
| `OUTLINE_SMTP_SECURE`      | No       | Defaults to `false`                                 |
| `OUTLINE_SMTP_FROM_EMAIL`  | Yes      | SMTP server from address.                           |
| `OUTLINE_SMTP_REPLY_EMAIL` | Yes      | SMTP server reply to address.                       |
