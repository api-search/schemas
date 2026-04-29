---
description: Kubernetes object metadata
layout: schema
name: ObjectMeta
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: generateName
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: uid
  type: string
- description: ''
  name: resourceVersion
  type: string
- description: ''
  name: generation
  type: integer
- description: ''
  name: creationTimestamp
  type: string
- description: ''
  name: labels
  type: object
- description: ''
  name: annotations
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-object-meta-schema.json
slug: argo-workflows-object-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-object-meta-schema.json\",\n  \"title\": \"ObjectMeta\",\n  \"description\": \"Kubernetes object metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"generateName\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"uid\": {\n      \"type\": \"string\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\"\n    },\n    \"generation\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"annotations\": {\n      \"type\": \"object\"\
  ,\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-object-meta-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: ObjectMeta
---
