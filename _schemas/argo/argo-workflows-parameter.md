---
description: A workflow parameter
layout: schema
name: Parameter
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: value
  type: string
- description: ''
  name: default
  type: string
- description: ''
  name: enum
  type: array
- description: ''
  name: description
  type: string
- description: ''
  name: globalName
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-parameter-schema.json
slug: argo-workflows-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-parameter-schema.json\",\n  \"title\": \"Parameter\",\n  \"description\": \"A workflow parameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"default\": {\n      \"type\": \"string\"\n    },\n    \"enum\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"globalName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-parameter-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Parameter
---
