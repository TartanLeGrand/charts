# clickhouse

![Version: 4.0.1](https://img.shields.io/badge/Version-4.0.1-informational?style=flat-square) ![AppVersion: 23.8.16.16](https://img.shields.io/badge/AppVersion-23.8.16.16-informational?style=flat-square)

ClickHouse is an open source column-oriented database management system capable of real time generation of analytical data reports using SQL queries

**Homepage:** <https://clickhouse.yandex/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| sentry-kubernetes |  |  |

## Source Code

* <https://github.com/sentry-kubernetes/charts>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| clickhouse.configmap.builtin_dictionaries_reload_interval | string | `"3600"` |  |
| clickhouse.configmap.compression.cases[0].method | string | `"zstd"` |  |
| clickhouse.configmap.compression.cases[0].min_part_size | string | `"10000000000"` |  |
| clickhouse.configmap.compression.cases[0].min_part_size_ratio | string | `"0.01"` |  |
| clickhouse.configmap.compression.enabled | bool | `false` |  |
| clickhouse.configmap.configOverride | string | `""` |  |
| clickhouse.configmap.default_session_timeout | string | `"60"` |  |
| clickhouse.configmap.disable_internal_dns_cache | string | `"1"` |  |
| clickhouse.configmap.enabled | bool | `true` |  |
| clickhouse.configmap.graphite.config[0].asynchronous_metrics | bool | `true` |  |
| clickhouse.configmap.graphite.config[0].events | bool | `true` |  |
| clickhouse.configmap.graphite.config[0].events_cumulative | bool | `true` |  |
| clickhouse.configmap.graphite.config[0].interval | string | `"60"` |  |
| clickhouse.configmap.graphite.config[0].metrics | bool | `true` |  |
| clickhouse.configmap.graphite.config[0].root_path | string | `"one_min"` |  |
| clickhouse.configmap.graphite.config[0].timeout | string | `"0.1"` |  |
| clickhouse.configmap.graphite.enabled | bool | `false` |  |
| clickhouse.configmap.keep_alive_timeout | string | `"3"` |  |
| clickhouse.configmap.logger.count | string | `"10"` |  |
| clickhouse.configmap.logger.level | string | `"trace"` |  |
| clickhouse.configmap.logger.path | string | `"/var/log/clickhouse-server"` |  |
| clickhouse.configmap.logger.size | string | `"1000M"` |  |
| clickhouse.configmap.logger.stdoutLogsEnabled | bool | `false` |  |
| clickhouse.configmap.mark_cache_size | string | `"5368709120"` |  |
| clickhouse.configmap.max_concurrent_queries | string | `"100"` |  |
| clickhouse.configmap.max_connections | string | `"4096"` |  |
| clickhouse.configmap.max_session_timeout | string | `"3600"` |  |
| clickhouse.configmap.merge_tree.enabled | bool | `false` |  |
| clickhouse.configmap.merge_tree.max_part_loading_threads | string | `"auto"` |  |
| clickhouse.configmap.merge_tree.max_suspicious_broken_parts | int | `100` |  |
| clickhouse.configmap.merge_tree.parts_to_delay_insert | int | `150` |  |
| clickhouse.configmap.merge_tree.parts_to_throw_insert | int | `300` |  |
| clickhouse.configmap.mlock_executable | bool | `false` |  |
| clickhouse.configmap.profiles.enabled | bool | `false` |  |
| clickhouse.configmap.profiles.profile[0].config.load_balancing | string | `"random"` |  |
| clickhouse.configmap.profiles.profile[0].config.max_memory_usage | string | `"10000000000"` |  |
| clickhouse.configmap.profiles.profile[0].config.use_uncompressed_cache | string | `"0"` |  |
| clickhouse.configmap.profiles.profile[0].name | string | `"default"` |  |
| clickhouse.configmap.quotas.enabled | bool | `false` |  |
| clickhouse.configmap.quotas.quota[0].config[0].duration | string | `"3600"` |  |
| clickhouse.configmap.quotas.quota[0].config[0].errors | string | `"0"` |  |
| clickhouse.configmap.quotas.quota[0].config[0].execution_time | string | `"0"` |  |
| clickhouse.configmap.quotas.quota[0].config[0].queries | string | `"0"` |  |
| clickhouse.configmap.quotas.quota[0].config[0].read_rows | string | `"0"` |  |
| clickhouse.configmap.quotas.quota[0].config[0].result_rows | string | `"0"` |  |
| clickhouse.configmap.quotas.quota[0].name | string | `"default"` |  |
| clickhouse.configmap.remote_servers.enabled | bool | `true` |  |
| clickhouse.configmap.remote_servers.internal_replication | bool | `false` |  |
| clickhouse.configmap.remote_servers.replica.backup.enabled | bool | `true` |  |
| clickhouse.configmap.remote_servers.replica.compression | bool | `true` |  |
| clickhouse.configmap.remote_servers.replica.user | string | `"default"` |  |
| clickhouse.configmap.umask | string | `"022"` |  |
| clickhouse.configmap.uncompressed_cache_size | string | `"8589934592"` |  |
| clickhouse.configmap.users.enabled | bool | `false` |  |
| clickhouse.configmap.users.user[0].config.networks[0] | string | `"::/0"` |  |
| clickhouse.configmap.users.user[0].config.profile | string | `"default"` |  |
| clickhouse.configmap.users.user[0].config.quota | string | `"default"` |  |
| clickhouse.configmap.users.user[0].name | string | `"default"` |  |
| clickhouse.configmap.zookeeper_servers.config[0].host | string | `""` |  |
| clickhouse.configmap.zookeeper_servers.config[0].index | string | `""` |  |
| clickhouse.configmap.zookeeper_servers.config[0].port | string | `""` |  |
| clickhouse.configmap.zookeeper_servers.enabled | bool | `false` |  |
| clickhouse.configmap.zookeeper_servers.operation_timeout_ms | string | `"10000"` |  |
| clickhouse.configmap.zookeeper_servers.session_timeout_ms | string | `"30000"` |  |
| clickhouse.http_port | string | `"8123"` |  |
| clickhouse.image | string | `"clickhouse/clickhouse-server"` |  |
| clickhouse.imagePullPolicy | string | `"IfNotPresent"` |  |
| clickhouse.imageVersion | string | `nil` |  |
| clickhouse.ingress.enabled | bool | `false` |  |
| clickhouse.interserver_http_port | string | `"9009"` |  |
| clickhouse.listen_host | string | `"0.0.0.0"` |  |
| clickhouse.livenessProbe.enabled | bool | `true` |  |
| clickhouse.livenessProbe.failureThreshold | int | `3` |  |
| clickhouse.livenessProbe.initialDelaySeconds | int | `0` |  |
| clickhouse.livenessProbe.periodSeconds | int | `30` |  |
| clickhouse.livenessProbe.successThreshold | int | `1` |  |
| clickhouse.livenessProbe.timeoutSeconds | int | `5` |  |
| clickhouse.metrics.enabled | bool | `true` |  |
| clickhouse.metrics.podAnnotations."prometheus.io/port" | string | `"9116"` |  |
| clickhouse.metrics.podAnnotations."prometheus.io/scrape" | string | `"true"` |  |
| clickhouse.metrics.port | int | `9116` |  |
| clickhouse.metrics.prometheusRule.additionalLabels | object | `{}` |  |
| clickhouse.metrics.prometheusRule.enabled | bool | `false` |  |
| clickhouse.metrics.prometheusRule.namespace | string | `""` |  |
| clickhouse.metrics.prometheusRule.rules | list | `[]` |  |
| clickhouse.metrics.service.annotations | object | `{}` |  |
| clickhouse.metrics.service.labels | object | `{}` |  |
| clickhouse.metrics.service.type | string | `"ClusterIP"` |  |
| clickhouse.metrics.serviceMonitor.enabled | bool | `false` |  |
| clickhouse.metrics.serviceMonitor.selector.prometheus | string | `"kube-prometheus"` |  |
| clickhouse.path | string | `"/var/lib/clickhouse"` |  |
| clickhouse.persistentVolumeClaim.dataPersistentVolume.accessModes[0] | string | `"ReadWriteOnce"` |  |
| clickhouse.persistentVolumeClaim.dataPersistentVolume.enabled | bool | `false` |  |
| clickhouse.persistentVolumeClaim.dataPersistentVolume.storage | string | `"500Gi"` |  |
| clickhouse.persistentVolumeClaim.enabled | bool | `false` |  |
| clickhouse.persistentVolumeClaim.logsPersistentVolume.accessModes[0] | string | `"ReadWriteOnce"` |  |
| clickhouse.persistentVolumeClaim.logsPersistentVolume.enabled | bool | `false` |  |
| clickhouse.persistentVolumeClaim.logsPersistentVolume.storage | string | `"50Gi"` |  |
| clickhouse.podManagementPolicy | string | `"Parallel"` |  |
| clickhouse.podSecurityContext | object | `{}` |  |
| clickhouse.priorityClassName | string | `nil` |  |
| clickhouse.readinessProbe.enabled | bool | `true` |  |
| clickhouse.readinessProbe.failureThreshold | int | `3` |  |
| clickhouse.readinessProbe.initialDelaySeconds | int | `0` |  |
| clickhouse.readinessProbe.periodSeconds | int | `30` |  |
| clickhouse.readinessProbe.successThreshold | int | `1` |  |
| clickhouse.readinessProbe.timeoutSeconds | int | `5` |  |
| clickhouse.replicas | string | `"3"` |  |
| clickhouse.resources | object | `{}` |  |
| clickhouse.securityContext | object | `{}` |  |
| clickhouse.startupProbe.enabled | bool | `true` |  |
| clickhouse.startupProbe.failureThreshold | int | `60` |  |
| clickhouse.startupProbe.periodSeconds | int | `5` |  |
| clickhouse.startupProbe.successThreshold | int | `1` |  |
| clickhouse.startupProbe.timeoutSeconds | int | `5` |  |
| clickhouse.tcp_port | string | `"9000"` |  |
| clickhouse.updateStrategy | string | `"RollingUpdate"` |  |
| clusterDomain | string | `"cluster.local"` |  |
| serviceAccount.annotations | object | `{}` | Additional Service Account annotations. |
| serviceAccount.automountServiceAccountToken | bool | `true` | Automount API credentials for a Service Account. |
| serviceAccount.enabled | bool | `false` | If `true`, a custom Service Account will be used. |
| serviceAccount.name | string | `"clickhouse"` | The name of the ServiceAccount to use. Will be appended with `replica` and `tabix` for those pods. |
| tabix.enabled | bool | `false` |  |
| tabix.image | string | `"spoonest/clickhouse-tabix-web-client"` |  |
| tabix.imagePullPolicy | string | `"IfNotPresent"` |  |
| tabix.imageVersion | string | `"stable"` |  |
| tabix.ingress.enabled | bool | `false` |  |
| tabix.livenessProbe.enabled | bool | `true` |  |
| tabix.livenessProbe.failureThreshold | string | `"3"` |  |
| tabix.livenessProbe.initialDelaySeconds | string | `"30"` |  |
| tabix.livenessProbe.periodSeconds | string | `"30"` |  |
| tabix.livenessProbe.successThreshold | string | `"1"` |  |
| tabix.livenessProbe.timeoutSeconds | string | `"5"` |  |
| tabix.podAnnotations | string | `nil` |  |
| tabix.podLabels | string | `nil` |  |
| tabix.readinessProbe.enabled | bool | `true` |  |
| tabix.readinessProbe.failureThreshold | string | `"3"` |  |
| tabix.readinessProbe.initialDelaySeconds | string | `"30"` |  |
| tabix.readinessProbe.periodSeconds | string | `"30"` |  |
| tabix.readinessProbe.successThreshold | string | `"1"` |  |
| tabix.readinessProbe.timeoutSeconds | string | `"5"` |  |
| tabix.replicas | string | `"1"` |  |
| tabix.resources | object | `{}` |  |
| tabix.security.password | string | `"admin"` |  |
| tabix.security.user | string | `"admin"` |  |
| tabix.updateStrategy.maxSurge | int | `3` |  |
| tabix.updateStrategy.maxUnavailable | int | `1` |  |
| tabix.updateStrategy.type | string | `"RollingUpdate"` |  |
| timezone | string | `"UTC"` |  |

