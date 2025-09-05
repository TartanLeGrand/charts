# sentry-kubernetes

![Version: 0.4.0](https://img.shields.io/badge/Version-0.4.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: latest](https://img.shields.io/badge/AppVersion-latest-informational?style=flat-square)

A Helm chart for sentry-kubernetes (https://github.com/getsentry/sentry-kubernetes)

**Homepage:** <https://github.com/getsentry/sentry-kubernetes>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| sentry-kubernetes |  |  |

## Source Code

* <https://github.com/getsentry/sentry-kubernetes>
* <https://github.com/sentry-kubernetes/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"ghcr.io/getsentry/sentry-kubernetes"` |  |
| image.tag | string | `"latest"` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| rbac.create | bool | `true` |  |
| resources | object | `{}` |  |
| sentry.dsn | string | `"<change-me>"` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `nil` |  |

