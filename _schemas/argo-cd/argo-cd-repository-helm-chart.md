---
description: repositoryHelmChart schema from Argo CD API
layout: schema
name: repositoryHelmChart
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: versions
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-helm-chart-schema.json
slug: argo-cd-repository-helm-chart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-chart-schema.json\",\n  \"title\": \"repositoryHelmChart\",\n  \"description\": \"repositoryHelmChart schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-chart-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryHelmChart
---
