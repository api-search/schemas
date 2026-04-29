---
description: A registered Kubernetes cluster deployment target.
layout: schema
name: Cluster
properties_list:
- description: Kubernetes API server URL.
  name: server
  type: string
- description: Cluster display name.
  name: name
  type: string
- description: Cluster connection configuration.
  name: config
  type: object
- description: Cluster information.
  name: info
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-cluster-schema.json
slug: argo-cd-cluster
source_filename: argo-cd-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-cluster-schema.json\",\n  \"title\": \"Cluster\",\n  \"description\": \"A registered Kubernetes cluster deployment target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"server\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes API server URL.\",\n      \"format\": \"uri\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster display name.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster connection configuration.\",\n      \"properties\": {\n        \"bearerToken\": {\n          \"type\": \"string\",\n          \"description\": \"Service account bearer token for cluster access.\"\n        },\n        \"tlsClientConfig\": {\n          \"type\": \"object\",\n          \"description\": \"TLS client configuration.\"\
  ,\n          \"properties\": {\n            \"insecure\": {\n              \"type\": \"boolean\",\n              \"description\": \"Skip TLS verification.\"\n            }\n          }\n        }\n      }\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster information.\",\n      \"properties\": {\n        \"serverVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes server version.\"\n        },\n        \"applicationsCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of applications targeting this cluster.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-cluster-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Cluster
---
