# magda

![Version: 1.1.0-alpha.2](https://img.shields.io/badge/Version-1.1.0--alpha.2-informational?style=flat-square)

A complete solution for managing, publishing and discovering government data, private and open. This chart includes the magda default deployment.

**Homepage:** <https://github.com/magda-io/magda>

## Source Code

* <https://github.com/magda-io/magda>

## Requirements

Kubernetes: `>= 1.14.0-0`

| Repository | Name | Version |
|------------|------|---------|
| file://../magda-core | magda-core | 1.1.0-alpha.2 |
| https://charts.magda.io | ckan-connector-functions(magda-ckan-connector) | 1.2.0 |
| https://charts.magda.io | magda-function-esri-url-processor | 1.0.0 |
| https://charts.magda.io | magda-function-history-report | 1.0.0 |
| https://charts.magda.io | minion-broken-link(magda-minion-broken-link) | 1.0.0 |
| https://charts.magda.io | magda-minion-ckan-exporter | 1.0.0 |
| https://charts.magda.io | minion-format(magda-minion-format) | 1.1.0 |
| https://charts.magda.io | minion-linked-data-rating(magda-minion-linked-data-rating) | 1.1.0 |
| https://charts.magda.io | minion-visualization(magda-minion-visualization) | 1.0.0 |
| https://charts.magda.io | openfaas | 5.5.5-magda |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| ckan-connector-functions.createConfigMap | bool | `false` |  |
| ckan-connector-functions.createFunction | bool | `true` |  |
| ckan-connector-functions.includeCronJobs | bool | `false` |  |
| ckan-connector-functions.includeInitialJobs | bool | `false` |  |
| global.connectors.includeCronJobs | bool | `true` |  |
| global.connectors.includeInitialJobs | bool | `false` |  |
| global.openfaas.allowAdminOnly | bool | `true` |  |
| global.openfaas.enabled | bool | `true` |  |
| global.openfaas.functionNamespace | string | `"openfaas-fn"` |  |
| global.openfaas.mainNamespace | string | `"openfaas"` |  |
| global.openfaas.namespacePrefix | string | `""` |  |
| global.openfaas.secrets.authSecrets | bool | `true` |  |
| openfaas.basic_auth | bool | `false` |  |
| openfaas.faasIdler.dryRun | bool | `false` |  |
| openfaas.faasnetes.imagePullPolicy | string | `"IfNotPresent"` |  |
| openfaas.faasnetes.readTimeout | string | `"120s"` |  |
| openfaas.faasnetes.writeTimeout | string | `"120s"` |  |
| openfaas.gateway.readTimeout | string | `"125s"` |  |
| openfaas.gateway.scaleFromZero | bool | `true` |  |
| openfaas.gateway.upstreamTimeout | string | `"120s"` |  |
| openfaas.gateway.writeTimeout | string | `"125s"` |  |
| openfaas.ingress.enabled | bool | `false` |  |
| openfaas.operator.create | bool | `true` |  |
| openfaas.serviceType | string | `"ClusterIP"` |  |
| tags.all | bool | `true` |  |
| tags.connectors | bool | `false` |  |
| tags.minion-broken-link | bool | `false` |  |
| tags.minion-ckan-exporter | bool | `false` |  |
| tags.minion-format | bool | `false` |  |
| tags.minion-linked-data-rating | bool | `false` |  |
| tags.minion-visualization | bool | `false` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
