# gke-preemptible-notifier

![Version: 0.0.5](https://img.shields.io/badge/Version-0.0.5-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.0.3](https://img.shields.io/badge/AppVersion-v0.0.3-informational?style=flat-square)

Helm chart to deploy [gke-preemptible-notifier](https://github.com/slamdev/gke-preemptible-notifier/).

**Homepage:** <https://github.com/slamdev/helm-charts/tree/master/charts/gke-preemptible-notifier>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| slamdev | valentin.fedoskin@gmail.com |  |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` | affinity for scheduler pod assignment |
| env | list | `[{"name":"GKE_PREEMPTIBLE_NOTIFIER_LOG_FORMAT","value":"json"}]` | environment variables for the container |
| envFrom | list | `[]` | environment variable sources for the container |
| fullnameOverride | string | `""` | full name of the chart. |
| image.pullPolicy | string | `"IfNotPresent"` | image pull policy |
| image.repository | string | `"slamdev/gke-preemptible-notifier"` | image repository |
| image.tag | string | `""` | image tag (chart's appVersion value will be used if not set) |
| imagePullSecrets | list | `[]` | image pull secret for private images |
| nameOverride | string | `""` | override name of the chart |
| nodeSelector | object | `{}` | node for scheduler pod assignment |
| podSecurityContext | object | `{}` | specifies security settings for a pod |
| resources | object | `{}` | custom resource configuration |
| securityContext | object | `{}` | specifies security settings for a container |
| serviceAccount.annotations | object | `{}` | annotations to add to the service account |
| serviceAccount.name | string | `nil` | the name of the service account to use; if not set, a name is generated using the fullname template |
| tolerations | list | `[]` | tolerations for scheduler pod assignment |
| volumeMounts | list | `[]` | additional volume mounts |
| volumes | list | `[]` | volumes |
