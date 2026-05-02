---
description: Schema for the values.yaml file in a Helm chart. The values.yaml file provides default configuration values for a chart. Values can be overridden during installation or upgrade using --set flags or additional values files. While the structure of values.yaml is chart-specific, this schema describes common conventional patterns used across the Helm ecosystem.
layout: schema
name: Helm Values YAML
properties_list:
- description: Number of pod replicas to deploy.
  name: replicaCount
  type: integer
- description: Container image configuration.
  name: image
  type: object
- description: Override the chart name used in resource names.
  name: nameOverride
  type: string
- description: Override the full resource name prefix.
  name: fullnameOverride
  type: string
- description: Service account configuration.
  name: serviceAccount
  type: object
- description: Annotations to add to the pod.
  name: podAnnotations
  type: object
- description: Labels to add to the pod.
  name: podLabels
  type: object
- description: Security context for the pod.
  name: podSecurityContext
  type: object
- description: Security context for the container.
  name: securityContext
  type: object
- description: Kubernetes Service configuration.
  name: service
  type: object
- description: Kubernetes Ingress configuration.
  name: ingress
  type: object
- description: CPU and memory resource requests and limits for the container.
  name: resources
  type: object
- description: Horizontal Pod Autoscaler configuration.
  name: autoscaling
  type: object
- description: Node labels for pod assignment.
  name: nodeSelector
  type: object
- description: Tolerations for pod scheduling.
  name: tolerations
  type: array
- description: Affinity rules for pod scheduling.
  name: affinity
  type: object
- description: Global values shared across all chart dependencies. These values are accessible to both the parent chart and all subcharts.
  name: global
  type: object
provider_name: Helm
provider_slug: helm
schema_file: json-schema/helm-values-yaml-schema.json
slug: helm-values-yaml
source_filename: helm-values-yaml-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://helm.sh/schemas/values-yaml.json\",\n  \"title\": \"Helm Values YAML\",\n  \"description\": \"Schema for the values.yaml file in a Helm chart. The values.yaml file provides default configuration values for a chart. Values can be overridden during installation or upgrade using --set flags or additional values files. While the structure of values.yaml is chart-specific, this schema describes common conventional patterns used across the Helm ecosystem.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"replicaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pod replicas to deploy.\",\n      \"minimum\": 0,\n      \"default\": 1\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"Container image configuration.\",\n      \"properties\": {\n        \"repository\": {\n          \"type\": \"string\",\n          \"description\": \"Container\
  \ image repository and name.\",\n          \"examples\": [\n            \"nginx\",\n            \"docker.io/library/nginx\"\n          ]\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"Container image tag. Defaults to the chart appVersion if empty.\"\n        },\n        \"pullPolicy\": {\n          \"type\": \"string\",\n          \"description\": \"Image pull policy for Kubernetes.\",\n          \"enum\": [\n            \"Always\",\n            \"IfNotPresent\",\n            \"Never\"\n          ],\n          \"default\": \"IfNotPresent\"\n        },\n        \"pullSecrets\": {\n          \"type\": \"array\",\n          \"description\": \"List of image pull secret names.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"nameOverride\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Override the chart name used in resource names.\"\n    },\n    \"fullnameOverride\": {\n      \"type\": \"string\",\n      \"description\": \"Override the full resource name prefix.\"\n    },\n    \"serviceAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Service account configuration.\",\n      \"properties\": {\n        \"create\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to create a service account.\",\n          \"default\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the service account. Auto-generated if not set.\"\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"description\": \"Annotations to add to the service account.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"automount\": {\n          \"type\": \"boolean\",\n    \
  \      \"description\": \"Whether to automount the service account token.\",\n          \"default\": true\n        }\n      }\n    },\n    \"podAnnotations\": {\n      \"type\": \"object\",\n      \"description\": \"Annotations to add to the pod.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"podLabels\": {\n      \"type\": \"object\",\n      \"description\": \"Labels to add to the pod.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"podSecurityContext\": {\n      \"type\": \"object\",\n      \"description\": \"Security context for the pod.\",\n      \"properties\": {\n        \"fsGroup\": {\n          \"type\": \"integer\"\n        },\n        \"runAsUser\": {\n          \"type\": \"integer\"\n        },\n        \"runAsGroup\": {\n          \"type\": \"integer\"\n        },\n        \"runAsNonRoot\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"securityContext\": {\n    \
  \  \"type\": \"object\",\n      \"description\": \"Security context for the container.\",\n      \"properties\": {\n        \"allowPrivilegeEscalation\": {\n          \"type\": \"boolean\"\n        },\n        \"capabilities\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"drop\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"add\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"readOnlyRootFilesystem\": {\n          \"type\": \"boolean\"\n        },\n        \"runAsNonRoot\": {\n          \"type\": \"boolean\"\n        },\n        \"runAsUser\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"service\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes Service configuration.\",\n      \"\
  properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes Service type.\",\n          \"enum\": [\n            \"ClusterIP\",\n            \"NodePort\",\n            \"LoadBalancer\",\n            \"ExternalName\"\n          ],\n          \"default\": \"ClusterIP\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"Service port number.\",\n          \"default\": 80\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"ingress\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes Ingress configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"className\": {\n          \"type\": \"string\",\n          \"description\": \"Ingress class name.\"\
  \n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"hosts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"host\": {\n                \"type\": \"string\"\n              },\n              \"paths\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"path\": {\n                      \"type\": \"string\"\n                    },\n                    \"pathType\": {\n                      \"type\": \"string\",\n                      \"enum\": [\n                        \"Exact\",\n                        \"Prefix\",\n                        \"ImplementationSpecific\"\n                      ]\n                    }\n                  }\n             \
  \   }\n              }\n            }\n          }\n        },\n        \"tls\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"secretName\": {\n                \"type\": \"string\"\n              },\n              \"hosts\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"CPU and memory resource requests and limits for the container.\",\n      \"properties\": {\n        \"limits\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cpu\": {\n              \"type\": \"string\",\n              \"examples\": [\"500m\", \"1\"]\n            },\n            \"memory\": {\n              \"type\": \"string\",\n              \"examples\": [\"128Mi\"\
  , \"512Mi\"]\n            }\n          }\n        },\n        \"requests\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cpu\": {\n              \"type\": \"string\",\n              \"examples\": [\"100m\", \"250m\"]\n            },\n            \"memory\": {\n              \"type\": \"string\",\n              \"examples\": [\"64Mi\", \"256Mi\"]\n            }\n          }\n        }\n      }\n    },\n    \"autoscaling\": {\n      \"type\": \"object\",\n      \"description\": \"Horizontal Pod Autoscaler configuration.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"minReplicas\": {\n          \"type\": \"integer\",\n          \"default\": 1\n        },\n        \"maxReplicas\": {\n          \"type\": \"integer\",\n          \"default\": 100\n        },\n        \"targetCPUUtilizationPercentage\": {\n          \"type\": \"integer\"\n        },\n        \"targetMemoryUtilizationPercentage\"\
  : {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\",\n      \"description\": \"Node labels for pod assignment.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tolerations\": {\n      \"type\": \"array\",\n      \"description\": \"Tolerations for pod scheduling.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"operator\": {\n            \"type\": \"string\",\n            \"enum\": [\"Exists\", \"Equal\"]\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"effect\": {\n            \"type\": \"string\",\n            \"enum\": [\"NoSchedule\", \"PreferNoSchedule\", \"NoExecute\"]\n          },\n          \"tolerationSeconds\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"affinity\":\
  \ {\n      \"type\": \"object\",\n      \"description\": \"Affinity rules for pod scheduling.\",\n      \"properties\": {\n        \"nodeAffinity\": {\n          \"type\": \"object\"\n        },\n        \"podAffinity\": {\n          \"type\": \"object\"\n        },\n        \"podAntiAffinity\": {\n          \"type\": \"object\"\n        }\n      }\n    },\n    \"global\": {\n      \"type\": \"object\",\n      \"description\": \"Global values shared across all chart dependencies. These values are accessible to both the parent chart and all subcharts.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/helm/refs/heads/main/json-schema/helm-values-yaml-schema.json
tags:
- Charts
- Cloud Native
- Container Orchestration
- DevOps
- Kubernetes
- Package Manager
title: Helm Values YAML
---
