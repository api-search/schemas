---
description: repositoryHelmChartsResponse schema from Argo CD API
layout: schema
name: repositoryHelmChartsResponse
properties_list:
- description: ''
  name: items
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-helm-charts-response-schema.json
slug: argo-cd-repository-helm-charts-response
source_filename: argo-cd-repository-helm-charts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-charts-response-schema.json\",\n  \"title\": \"repositoryHelmChartsResponse\",\n  \"description\": \"repositoryHelmChartsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/repositoryHelmChart\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-repository-helm-charts-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryHelmChartsResponse
---
