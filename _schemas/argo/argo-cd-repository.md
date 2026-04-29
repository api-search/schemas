---
description: A registered Git or Helm chart repository.
layout: schema
name: Repository
properties_list:
- description: Repository URL.
  name: repo
  type: string
- description: Repository type.
  name: type
  type: string
- description: Human-readable repository name.
  name: name
  type: string
- description: Current connection status.
  name: connectionState
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-repository-schema.json
slug: argo-cd-repository
source_filename: argo-cd-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"A registered Git or Helm chart repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repo\": {\n      \"type\": \"string\",\n      \"description\": \"Repository URL.\",\n      \"format\": \"uri\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Repository type.\",\n      \"enum\": [\n        \"git\",\n        \"helm\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable repository name.\"\n    },\n    \"connectionState\": {\n      \"type\": \"object\",\n      \"description\": \"Current connection status.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Connection status\
  \ (Successful, Failed, Unknown).\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Status message.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-repository-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Repository
---
