---
description: clusterDexConfig schema from Argo CD API
layout: schema
name: clusterDexConfig
properties_list:
- description: ''
  name: connectors
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-cluster-dex-config-schema.json
slug: argo-cd-cluster-dex-config
source_filename: argo-cd-cluster-dex-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-dex-config-schema.json\",\n  \"title\": \"clusterDexConfig\",\n  \"description\": \"clusterDexConfig schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/clusterConnector\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-cluster-dex-config-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: clusterDexConfig
---
