# stressed-pod

![Version: 1.0.1](https://img.shields.io/badge/Version-1.0.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.2](https://img.shields.io/badge/AppVersion-1.0.2-informational?style=flat-square)

A Helm chart for deploying Stressed Pod - a Kubernetes pod testing tool

**Homepage:** <https://github.com/SQuent/helm-charts>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Quentin SALLIO | <q.sallio@gmail.com> |  |

## Source Code

* <https://github.com/SQuent/stressed-pod>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| config.cpuLoad.dynamic.duration | int | `60` |  |
| config.cpuLoad.dynamic.enabled | bool | `false` |  |
| config.cpuLoad.dynamic.final | float | `0.5` |  |
| config.cpuLoad.dynamic.initial | int | `0` |  |
| config.cpuLoad.dynamic.stopAtEnd | bool | `true` |  |
| config.cpuLoad.enabled | bool | `false` |  |
| config.logging.duration | int | `60` |  |
| config.logging.enabled | bool | `false` |  |
| config.logging.format | string | `"json"` |  |
| config.logging.interval | int | `5` |  |
| config.logging.level | string | `"info"` |  |
| config.logging.message | string | `"Automatic log message"` |  |
| config.logging.service | string | `"auto-logger"` |  |
| config.memoryLoad.dynamic.duration | int | `60` |  |
| config.memoryLoad.dynamic.enabled | bool | `false` |  |
| config.memoryLoad.dynamic.final | int | `256` |  |
| config.memoryLoad.dynamic.initial | int | `0` |  |
| config.memoryLoad.dynamic.stopAtEnd | bool | `true` |  |
| config.memoryLoad.enabled | bool | `false` |  |
| config.probes.livenessStatus | string | `"SUCCESS"` |  |
| config.probes.readinessStatus | string | `"SUCCESS"` |  |
| config.system.autoTermination.delay | int | `300` |  |
| config.system.autoTermination.enabled | bool | `false` |  |
| deployment.replicas | int | `1` |  |
| deployment.resources.limits.cpu | string | `"1000m"` |  |
| deployment.resources.limits.memory | string | `"512Mi"` |  |
| deployment.resources.requests.cpu | string | `"100m"` |  |
| deployment.resources.requests.memory | string | `"128Mi"` |  |
| fullnameOverride | string | `""` |  |
| hpa.enabled | bool | `true` |  |
| hpa.maxReplicas | int | `5` |  |
| hpa.minReplicas | int | `1` |  |
| hpa.targetCPUUtilizationPercentage | int | `80` |  |
| hpa.targetMemoryUtilizationPercentage | int | `80` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/squent/stressed-pod"` |  |
| nameOverride | string | `""` |  |
| service.port | int | `8000` |  |
| service.type | string | `"ClusterIP"` |  |

