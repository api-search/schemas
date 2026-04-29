---
description: A Workload represents a Kubernetes workload monitored by CAST AI for optimization, including resource requests and recommendations.
layout: schema
name: CAST AI Workload
properties_list:
- description: Unique identifier for the workload.
  name: id
  type: string
- description: ID of the cluster the workload belongs to.
  name: clusterId
  type: string
- description: Kubernetes namespace of the workload.
  name: namespace
  type: string
- description: Name of the workload.
  name: name
  type: string
- description: Kubernetes workload type.
  name: type
  type: string
- description: Containers within the workload.
  name: containers
  type: array
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/workload.json
slug: workload
source_filename: workload.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/workload.json\",\n  \"title\": \"CAST AI Workload\",\n  \"description\": \"A Workload represents a Kubernetes workload monitored by CAST AI for optimization, including resource requests and recommendations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the workload.\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the cluster the workload belongs to.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace of the workload.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workload.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n     \
  \ \"enum\": [\n        \"Deployment\",\n        \"StatefulSet\",\n        \"DaemonSet\",\n        \"Job\",\n        \"CronJob\"\n      ],\n      \"description\": \"Kubernetes workload type.\"\n    },\n    \"containers\": {\n      \"type\": \"array\",\n      \"description\": \"Containers within the workload.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the container.\"\n          },\n          \"requests\": {\n            \"type\": \"object\",\n            \"description\": \"Current resource requests for the container.\",\n            \"properties\": {\n              \"cpu\": {\n                \"type\": \"string\",\n                \"description\": \"CPU resource request (e.g., 100m, 1).\"\n              },\n              \"memory\": {\n                \"type\": \"string\",\n                \"description\": \"Memory resource request (e.g., 128Mi, 1Gi).\"\
  \n              }\n            }\n          },\n          \"recommendations\": {\n            \"type\": \"object\",\n            \"description\": \"CAST AI recommended resource values for the container.\",\n            \"properties\": {\n              \"cpu\": {\n                \"type\": \"string\",\n                \"description\": \"Recommended CPU resource request.\"\n              },\n              \"memory\": {\n                \"type\": \"string\",\n                \"description\": \"Recommended memory resource request.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/workload.json
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Workload
---
