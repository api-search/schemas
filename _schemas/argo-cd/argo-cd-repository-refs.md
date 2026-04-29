---
description: repositoryRefs schema from Argo CD API
layout: schema
name: repositoryRefs
properties_list:
- description: ''
  name: branches
  type: array
- description: ''
  name: tags
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-refs-schema.json
slug: argo-cd-repository-refs
source_filename: argo-cd-repository-refs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-refs-schema.json\",\n  \"title\": \"repositoryRefs\",\n  \"description\": \"repositoryRefs schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branches\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-refs-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryRefs
---
