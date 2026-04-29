---
description: InfoResponse schema from Argo API
layout: schema
name: InfoResponse
properties_list:
- description: The namespace managed by this Argo server
  name: managedNamespace
  type: string
- description: ''
  name: links
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-info-response-schema.json
slug: argo-workflows-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-info-response-schema.json\",\n  \"title\": \"InfoResponse\",\n  \"description\": \"InfoResponse schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"managedNamespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace managed by this Argo server\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"scope\": {\n            \"type\": \"string\"\n          },\n          \"url\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-info-response-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: InfoResponse
---
