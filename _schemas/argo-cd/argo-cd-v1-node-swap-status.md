---
description: NodeSwapStatus represents swap memory information.
layout: schema
name: v1NodeSwapStatus
properties_list:
- description: ''
  name: capacity
  type: integer
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-node-swap-status-schema.json
slug: argo-cd-v1-node-swap-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-node-swap-status-schema.json\",\n  \"title\": \"v1NodeSwapStatus\",\n  \"description\": \"NodeSwapStatus represents swap memory information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"Total amount of swap memory in bytes.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-node-swap-status-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1NodeSwapStatus
---
