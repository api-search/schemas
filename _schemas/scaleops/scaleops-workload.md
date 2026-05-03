---
description: A Kubernetes workload managed by ScaleOps for autonomous resource optimization
layout: schema
name: ScaleOps Workload
properties_list:
- description: Workload name (Kubernetes resource name)
  name: name
  type: string
- description: Kubernetes namespace containing the workload
  name: namespace
  type: string
- description: Kubernetes workload type
  name: kind
  type: string
- description: Kubernetes cluster identifier
  name: cluster
  type: string
- description: Container configurations within the workload
  name: containers
  type: array
- description: Replica scaling configuration
  name: replicas
  type: object
- description: Current ScaleOps optimization status
  name: optimization_status
  type: string
- description: Current estimated monthly cost in USD
  name: monthly_cost_current
  type: number
- description: Estimated monthly cost after optimization in USD
  name: monthly_cost_optimized
  type: number
- description: Estimated monthly savings from optimization in USD
  name: monthly_savings
  type: number
provider_name: ScaleOps
provider_slug: scaleops
schema_file: json-schema/scaleops-workload-schema.json
slug: scaleops-workload
source_filename: scaleops-workload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scaleops/main/json-schema/scaleops-workload-schema.json\",\n  \"title\": \"ScaleOps Workload\",\n  \"description\": \"A Kubernetes workload managed by ScaleOps for autonomous resource optimization\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"namespace\", \"kind\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workload name (Kubernetes resource name)\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace containing the workload\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"Deployment\", \"StatefulSet\", \"DaemonSet\", \"Job\", \"CronJob\"],\n      \"description\": \"Kubernetes workload type\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes cluster identifier\"\
  \n    },\n    \"containers\": {\n      \"type\": \"array\",\n      \"description\": \"Container configurations within the workload\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Container name\"\n          },\n          \"current_resources\": {\n            \"type\": \"object\",\n            \"description\": \"Current resource configuration\",\n            \"properties\": {\n              \"requests\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"cpu\": {\n                    \"type\": \"string\",\n                    \"description\": \"CPU request (e.g., 100m, 0.5)\"\n                  },\n                  \"memory\": {\n                    \"type\": \"string\",\n                    \"description\": \"Memory request (e.g., 128Mi, 1Gi)\"\n                  }\n                }\n              },\n              \"\
  limits\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"cpu\": {\n                    \"type\": \"string\"\n                  },\n                  \"memory\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"recommended_resources\": {\n            \"type\": \"object\",\n            \"description\": \"ScaleOps recommended resource configuration\",\n            \"properties\": {\n              \"requests\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"cpu\": {\n                    \"type\": \"string\"\n                  },\n                  \"memory\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"limits\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"cpu\": {\n       \
  \             \"type\": \"string\"\n                  },\n                  \"memory\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"actual_usage\": {\n            \"type\": \"object\",\n            \"description\": \"Observed actual resource usage\",\n            \"properties\": {\n              \"cpu_avg\": {\n                \"type\": \"string\",\n                \"description\": \"Average CPU usage\"\n              },\n              \"cpu_p95\": {\n                \"type\": \"string\",\n                \"description\": \"95th percentile CPU usage\"\n              },\n              \"memory_avg\": {\n                \"type\": \"string\"\n              },\n              \"memory_p95\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"replicas\": {\n      \"type\": \"object\",\n      \"description\": \"Replica scaling\
  \ configuration\",\n      \"properties\": {\n        \"current\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"recommended\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"min\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"max\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"optimization_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"optimized\", \"pending\", \"not_applicable\", \"excluded\"],\n      \"description\": \"Current ScaleOps optimization status\"\n    },\n    \"monthly_cost_current\": {\n      \"type\": \"number\",\n      \"description\": \"Current estimated monthly cost in USD\"\n    },\n    \"monthly_cost_optimized\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated monthly cost after optimization in USD\"\n    },\n    \"monthly_savings\": {\n      \"type\": \"number\",\n \
  \     \"description\": \"Estimated monthly savings from optimization in USD\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scaleops/refs/heads/main/json-schema/scaleops-workload-schema.json
tags:
- Azure
- Cost Optimization
- FinOps
- GCP
- Helm
- Kubernetes
- Resource Management
title: ScaleOps Workload
---
